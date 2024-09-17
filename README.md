# Node Scheduler Helper

**SchedulerHelper** is a utility class for managing cron job expressions in Node.js. It provides predefined cron expressions for common schedules like seconds, minutes, hours, daily, weekly, and more, making it easier to manage recurring tasks in your Node.js applications.



## Usage

Import and use the `SchedulerHelper` class to get cron expressions for your jobs:

```typescript
import SchedulerHelper from './SchedulerHelper';

// Example: Run a task every minute
const cronExpression = SchedulerHelper.everyMinute();
console.log(cronExpression); // Output: '0 * * * *'

// Example: Run a task daily at a specific time
const dailyTask = SchedulerHelper.dailyAt('14:30');
console.log(dailyTask); // Output: '30 14 * * *'
```

## Methods

- **everySecond()**: Runs every second.
- **everyTwoSeconds()**: Runs every two seconds.
- **everyMinute()**: Runs every minute.
- **hourly()**: Runs every hour.
- **daily()**: Runs every day at midnight.
- **weekly()**: Runs every week on Sunday at midnight.
- **monthly()**: Runs on the first day of every month at midnight.
- **yearly()**: Runs on the first day of every year at midnight.

And many more methods for customized scheduling.

## Inspiration

This project is inspired by [Laravel's scheduling options](https://laravel.com/docs/11.x/scheduling#schedule-frequency-options). It aims to bring a similar level of ease to Node.js applications.

## Contributing

If you find any issues or want to enhance the functionality, feel free to open a pull request (PR). Contributions are always welcome!

## License

This project is licensed under the MIT License.
