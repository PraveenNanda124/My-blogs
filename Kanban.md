# Kanban

![a](https://user-images.githubusercontent.com/116082827/235103717-ff687d8d-1cb0-487d-8038-7b61537433cf.png)


Kanban is an Agile methodology that emphasizes visualizing the workflow and limiting work in progress (WIP). The team uses a Kanban board to track the status of tasks, from the initial request to completion. Tasks are pulled from a backlog and moved through the board based on their status.

Sample code snippet for Kanban:



public class KanbanBoard {

    private List<Task> backlog;

    private List<Task> todo;

    private List<Task> inProgress;

    private List<Task> done;

    // Constructors, getters, and setters

}

public class Task {

    private String name;

    private String description;

    private int estimatedTime;

    private int remainingTime;

    private TaskStatus status;

    // Constructors, getters, and setters

}

public enum TaskStatus {

    BACKLOG,

    TODO,

    IN_PROGRESS,

    DONE

}
