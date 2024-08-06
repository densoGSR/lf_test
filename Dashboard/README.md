## Xronos Dashboard Test
Use some simple Lingua Franca programs to test whether the dashboard can visualize the expected software behavior

Checkpoint
- Reactor Run Order
- Reaction execution time

## Test Program

| LF Test code | Description | Diagram |
|----|----|----|
| [Single_Tread.lf](https://github.com/densoGSR/lf_test/blob/main/Dashboard/src/Single_Thread.lf)     | Test Single Thread LF program | ![Single_Thread][def]         |
| [Multi_Tread.lf](https://github.com/densoGSR/lf_test/blob/main/Dashboard/src/Multi_Thread.lf)     | Test Multi Thread LF program | ![Multi_Thread](https://github.com/densoGSR/lf_test/blob/main/Dashboard/doc/pic/Multi_Thread.png)        |
| [Timer.lf](https://github.com/densoGSR/lf_test/blob/main/Dashboard/src/Timer.lf)     | A simple test program that runs the sensor reactor periodically and displays the sensor output in the print reactor. | ![Timer](https://github.com/densoGSR/lf_test/blob/main/Dashboard/doc/pic/Timer.png)       |

## Test Instruction

Run Xronos-Dashboard
- See: [Xronos-Dashboard](https://github.com/xronos-inc/xronos-dashboard/tree/main)

Compile LF file
```sh
lfc src/Single_Thread.lf
```

Docker Run 
```sh
docker run --network xronos-dashboard --rm -it single_thread-main
```
Grafana
- host: `http://localhost:3000`
- username: `admin`
- password: `linguafranca`

## Test Result

Single Thread
![Single](https://github.com/densoGSR/lf_test/blob/main/Dashboard/doc/pic/Single_Thread_Result.png)

Multi Thread
![Multi](https://github.com/densoGSR/lf_test/blob/main/Dashboard/doc/pic/Multi_Thread_Result.png)

Timer
![Timer](https://github.com/densoGSR/lf_test/blob/main/Dashboard/doc/pic/Timer_Result.png)

[def]: https://github.com/densoGSR/lf_test/blob/main/Dashboard/doc/pic/Single_Thread.png