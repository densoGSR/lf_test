## Xronos Dashboard Test

| LF Test code | Description | Diagram |
|----|----|----|
| Single_Tread.lf     | This        | ![Single_Thread][def]         |
| Multi_Tread.lf     | This        | This         |

## Test Instruction

Run Xronos-Dashboard

Compile LF file
```sh
lfc src/Single_Thread.lf
```

Docker Run 
```sh
docker run --network xronos-dashboard --rm -it single_thread-main
```


[def]: https://github.com/densoGSR/lf_test/blob/main/Dashboard/doc/pic/Single_Thread.png