# etask_serial_clock

This package contains the code to output the time to the serial console every second

## Example excerpt

~~~c
#include <etask_serial_clock.h>

TaskHandle_t serial_clock_task;

void setup() {
  ...
  // Create a task to check and get OTA updates from S3
  xTaskCreate(
    etask_serial_clock,
    "Serial_Clock_Task",
    2000,
    NULL,
    0,
    &serial_clock_task
  );
}
~~~
