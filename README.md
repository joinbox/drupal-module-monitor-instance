# Monitor-Instance
The Joinbox Monitoring tool consists of the following two parts.
- [Monitor](https://github.com/joinbox/d9-module-monitor)
- [Instance](https://github.com/joinbox/d9-module-monitor-instance)

When instance is enabled it sends data to the monitor as soon as the Drupal Cron hook is triggered.

## Activation
Add the following lines to your settings.php file to enable functionality.
<br/>
- **Project**: This also is the identifier for the monitor. It should be the same project wide.
- **Environment**: Make sure to use _Live_, _Integration_ or _Stage_
```php
$settings['instance'] = [
  'project' => 'Instance',
  'environment' => 'Live'
  'monitor' => 'https://monitor.joinbox.com',
  'user' => 'monitor',
  'password' => 'monitor',
];
```
