# Queuing System in JS

## Table of Contents
- [Project Overview](#project-overview)
- [Technologies Used](#technologies-used)
- [Tasks](#tasks)
  - [Task 0: Simple Queue](#task-0-simple-queue)
  - [Task 1: Push Notification Queue](#task-1-push-notification-queue)
  - [Task 2: Kue Queue](#task-2-kue-queue)
  - [Task 3: Job Creator](#task-3-job-creator)
  - [Task 4: Job Processor](#task-4-job-processor)
  - [Task 5: Push Notification Job Processor](#task-5-push-notification-job-processor)
  - [Task 6: Push Notification Job Processing](#task-6-push-notification-job-processing)
  - [Task 7: Push Notification Job Error Handling](#task-7-push-notification-job-error-handling)
  - [Task 8: Job Creation Testing](#task-8-job-creation-testing)
  - [Task 9: Stock Management](#task-9-stock-management)
  - [Task 10: Seat Reservation](#task-10-seat-reservation)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

This project is designed to implement a queuing system using **JavaScript** for managing background jobs, reservations, and notifications. It utilizes **Redis** for data storage, **Kue** for job management, and **Express** for the web server to expose APIs that handle different tasks such as reserving seats, stock management, and sending push notifications.

The project covers multiple tasks that gradually build up an application capable of queuing, processing, and managing jobs and reservations.

## Technologies Used

- **JavaScript (ES6)**
- **Node.js**
- **Express**: For creating the web server and API endpoints.
- **Kue**: For managing job queues.
- **Redis**: For storing data like available seats, reservations, and stock information.
- **Mocha/Chai**: For testing purposes.
- **Util**: For promisifying Redis methods.

## Tasks

### Task 0: Simple Queue
- Create a simple queue system using **Kue** and **Redis**.
- This task covers the basics of adding and processing jobs.

### Task 1: Push Notification Queue
- Set up a queue specifically for managing **push notifications**.
- Create a job that sends notifications and processes them.

### Task 2: Kue Queue
- Create a queue using **Kue** to handle asynchronous jobs.
- Set up job creation and completion logic.

### Task 3: Job Creator
- Implement a function that can create jobs dynamically.
- This task ensures the queue can accept jobs and process them.

### Task 4: Job Processor
- Write the job processor that handles the jobs added to the queue.
- This task focuses on processing jobs with specific logic (e.g., sending notifications).

### Task 5: Push Notification Job Processor
- Implement a push notification job processor that handles notifications in the background.
- Add logic for job failure and success handling.

### Task 6: Push Notification Job Processing
- Modify the job processor to handle push notifications and simulate delays in processing.
- This task covers error handling during job execution.

### Task 7: Push Notification Job Error Handling
- Add robust error handling and logging to ensure job failures are properly captured and logged.
- This will ensure that job failures do not break the system.

### Task 8: Job Creation Testing
- Write tests to ensure job creation works as expected.
- Use **Mocha** and **Chai** for testing job creation and job handling in the queue.

### Task 9: Stock Management
- Set up stock management for a product inventory system.
- Implement API routes to manage product availability, reservations, and stock levels.

### Task 10: Seat Reservation
- Set up a seat reservation system that allows users to reserve seats through an Express API.
- Use Redis to manage seat availability and a Kue queue to process seat reservations asynchronously.

## Installation

To get started with this project, follow the steps below:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/harystyleseze/alx-backend.git
   ```

2. **Navigate to the project directory**:
   ```bash
   cd alx-backend/0x03-queuing_system_in_js
   ```

3. **Install dependencies**:
   ```bash
   npm install
   ```

4. **Install Redis**:
   - Ensure Redis is installed and running on your local machine or use a Redis cloud service.
   - [Redis Installation Guide](https://redis.io/download)

## Usage

### Running the Server

To start the server, use the following command:

```bash
npm run dev <filename.js>
```

For example, to run **task 10** (Seat Reservation), use:

```bash
npm run dev 100-seat.js
```

### Testing

This project includes **Mocha** and **Chai** for testing purposes. To run the tests, use:

```bash
npm test <test-file.js>
```

For example, to run tests for task 8 (Job Creation Testing):

```bash
npm test 8-job.test.js
```

## Contributing

If you would like to contribute to this project, please follow these steps:

1. Fork the repository.
2. Create a new branch for your changes.
3. Commit your changes and push them to your forked repository.
4. Create a pull request with a description of your changes.

## License

This project is licensed under the MIT License

---

### Contact Information:

- **Name**: Harrison Eze
- **Username**: harystyleseze
- **GitHub Profile**: [https://github.com/harystyleseze](https://github.com/harystyleseze)

