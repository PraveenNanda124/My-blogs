# Vector API

![j](https://user-images.githubusercontent.com/116082827/236687802-6a7a9467-dbc6-47eb-adc3-e125a4fd277d.jpeg)


Java 16 introduced a new Vector API that enables developers to perform mathematical operations on vectors of floating-point and integer values using hardware acceleration. This feature is designed to improve the performance of scientific and engineering applications.

Example:





VectorSpecies<Float> species = VectorSpecies.of(Float.TYPE, VectorShape.forSize(4));

float[] data = new float[] {1.0f, 2.0f, 3.0f, 4.0f};

var vec = species.fromArray(data, 0);

vec = vec.add(vec);

float[] result = vec.toArray();
