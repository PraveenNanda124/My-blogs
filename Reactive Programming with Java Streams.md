# Reactive Programming with Java Streams

![s](https://github.com/PraveenNanda124/Technical-blogs/assets/116082827/b97f5aaf-ea5f-406e-b2ba-69aada8a1403)


Java Streams provide a powerful way to process collections of data. Reactive programming takes it a step further by allowing you to build asynchronous and non-blocking applications. Here's an example using the Reactor library:



Flux<Integer> numbers = Flux.just(1, 2, 3, 4, 5);

numbers

    .map(n -> n * 2)

    .filter(n -> n > 5)

    .subscribe(System.out::println);
