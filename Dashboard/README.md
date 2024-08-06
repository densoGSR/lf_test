## Xronos Dashboard Test

| LF Test code | Description | Diagram |
|----|----|----|
| [Timer.lf](https://github.com/densoGSR/lf_test/tree/main/Dashboard/src/Timer.lf) | Test Simple Example | ![Timer](https://github.com/densoGSR/lf_test/tree/main/Dashboard/doc/pic/Timer.png) |
| [Single_Tread.lf](https://github.com/densoGSR/lf_test/blob/main/Dashboard/src/Single_Thread.lf)     | Test Single Thread LF program | ![Single_Thread][def]         |
| [Multi_Tread.lf](https://github.com/densoGSR/lf_test/blob/main/Dashboard/src/Multi_Thread.lf)     | Test Multi Thread LF program | ![Multi_Thread](https://github.com/densoGSR/lf_test/blob/main/Dashboard/doc/pic/Multi_Thread.png)        |

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


[def]: https://github.com/densoGSR/lf_test/blob/main/Dashboard/doc/pic/Single_Thread.png