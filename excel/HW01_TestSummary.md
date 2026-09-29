# Test Summary — Sharp KC-A70-W

**SUT:** SHARP KC-A70-W humidifying air purifier (2012)  
**Tester:** Nguyen Duc Quang / 20120359

## Counts

| Item | Count |
| --- | ---: |
| Total TCs | 15 |
| AI reviewed | 12 (TC01–TC12) |
| Student edges | 3 (TC13–TC15) |
| Videos shot | **6** — all **Pass** |
| Executed Pass | 6 (TC01,02,03,04,07,14) |
| Failed | 0 |
| Not run | 9 |

## Student edges (AI missed)

1. **TC13** Low/empty water → humidify warning  
2. **TC14** Power interrupt mid-run *(có trong bộ video)*  
3. **TC15** Intake briefly blocked  

## 6 TCs đã chọn quay video

| # | TC | Nói gì (~15–40s) |
| --- | --- | --- |
| 1 | **TC01** Power ON | Bấm nguồn → panel/gió |
| 2 | **TC02** Power OFF | Tắt máy → dừng |
| 3 | **TC03** Humidity % | Chỉ số độ ẩm |
| 4 | **TC04** Đèn nước / tạo ẩm | Chỉ đèn 加湿中 |
| 5 | **TC07** Airflow outlet | Tay gần miệng thổi |
| 6 | **TC14** Power interrupt | Đang chạy → rút phích → cắm lại + bật |

## Safety note (VN)

Máy rated **100 V**. Chỉ chạy khi nguồn/adapter phù hợp; không tự ý cắm 220 V trực tiếp.
