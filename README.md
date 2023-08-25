# freertos_counting_semaphore
Project Description: FreeRTOS Counting Semaphore for LCD Tasks

Introduction:
The project aims to implement a counting semaphore in the FreeRTOS (Real-Time Operating System) environment to facilitate the coordination of two tasks responsible for displaying information on an LCD screen. By utilizing the counting semaphore, the tasks can efficiently share and synchronize access to the LCD resources, ensuring proper sequencing and preventing conflicts.

Project Goals:

Task Division: Divide the LCD-related functionalities into two separate tasks to promote modularity and improve code organization.
Semaphore Implementation: Create a counting semaphore to control access to the LCD resources, allowing only one task at a time to modify or update the LCD display.
Task Synchronization: Utilize the counting semaphore to synchronize the execution of the LCD tasks, ensuring that they do not interfere with each other and maintain a consistent display state.
Efficiency and Responsiveness: Optimize the system to ensure efficient resource utilization and minimize the response time for LCD updates, providing a smooth and responsive user experience.

Project Components:

1- Counting Semaphore: Design and implement a counting semaphore that allows only one task to access the LCD resources at a time. The semaphore will maintain a count of available resources and block the tasks if the semaphore count reaches zero, ensuring proper synchronization.

2- LCD Task 1: Develop a task responsible for displaying dynamic information on the LCD screen. This task will acquire the counting semaphore, update the LCD display with the relevant data, and release the semaphore once the operation is complete.

3- LCD Task 2: Implement a second task that periodically updates the LCD screen with static information or system status. Similar to Task 1, this task will acquire the semaphore, perform the necessary LCD updates, and release the semaphore.
