# Extreme Programming (XP)

![a](https://user-images.githubusercontent.com/116082827/235159490-b5938778-48f4-4ae1-8342-112dbfe2959a.jpeg)


XP is an Agile methodology that emphasizes software quality and customer satisfaction. It involves practices such as test-driven development (TDD), continuous integration (CI), and pair programming. The team works closely with the customer to ensure that the software meets their needs.

Sample code snippet for XP:



public class Test {

    public void testAdd() {

        Calculator calc = new Calculator();

        int result = calc.add(2, 3);

        assertEquals(5, result);

    }

}

public class Calculator {

    public int add(int x, int y) {

        return x + y;

    }

}

public class ContinuousIntegration {

    public void build() {

        // Compile and run tests

        // Deploy to staging environment

        // Send notification to team

    }

}

public class PairProgramming {

    public void pairProgram()
