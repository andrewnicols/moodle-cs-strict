Moodle Coding Style with added Best Practice
============================================

This is an extended version of the (Moodle Coding style)[https://docs.moodle.org/dev/Coding_style] with added opinionated best practices.

## Installation
### Via Composer

```
composer global require andrewnicols/moodle-cs-strict
```

## Configuration

Note: This configuration depends on MDL-76272 having landed

1. Create a new `.phpcs.xml` file in your repository with the content:
```
<?xml version="1.0" encoding="UTF-8"?>
<ruleset name="MoodleCore">
  <rule ref="./phpcs.xml"/>
  <rule ref="MoodleStrict"/>
</ruleset>
```
