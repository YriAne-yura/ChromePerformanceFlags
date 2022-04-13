
# Chrome Optimizations Lag Fix
Để Chỉnh Sửa Và Cài Đặt Vui Lòng Vào Đây `chrome://flags`
* Lưu ý : Trong Đây Đều Là Tiếng Việt Được Dịch bởi 70-80% Bởi Google Dịch ( 20%-30% Do WDLF Dịch )
* My Channel: `https://www.youtube.com/channel/UC-FKTqZu2tO0-vgAM1S6dfw` ( Vietnamese ) 

## Tăng Hiệu Suất

<details><summary>Enabled</summary><p>

* #back-forward-cache - **bật bắt buộc lưu vào bộ nhớ đệm tất cả các trang (thử nghiệm)**
	* Đảm bảo rằng bạn đang sử dụng Flags
* #enable-parallel-downloading
* #enable-skia-renderer
* #enable-quic
* #enable-throttle-display-none-and-visibility-hidden-cross-origin-iframes
* #enable-vulkan - Disabled, nên vì do gây ra các trang web đen hoàn toàn và làm cho trình duyệt bị lag
	* Chức năng này được bật theo mặc định trên một số / hầu hết các thiết bị
                * Nếu bạn không gặp phải vấn đề tương tự, hãy giữ chức năng này làm mặc định
* #enable-webassembly-lazy-compilation
	* Chức năng là giả dược khi chế độ JITLess và chế độ Bảo mật nghiêm ngặt trong MS Edge được kích hoạt
* #overlay-strategies - **Bộ đệm đã bao gồm và không bao gồm (toàn màn hình, một trên trên, lớp dưới)**
	* Sử dụng chức năng này cho thế hệ Skylake hoặc mới hơn
* #subframe-shutdown-delay
* #throttle-foreground-timers

**Chức năng này không dành cho mọi thiết bị nhưng nó đáng để trải nghiệm thử**

Forcing them might be a bad idea. Therefore, before using them, please check out the Problems section by typing `chrome://gpu` into the address bar (ignore WebGL errors)
Dịch google: Buộc họ có thể là một ý tưởng tồi. Do đó, trước khi sử dụng chúng, vui lòng kiểm tra phần Sự cố bằng cách nhập `chrome: // gpu` vào thanh địa chỉ (bỏ qua lỗi WebGL)

* #enable-gpu-rasterization
* #enable-zero-copy
* #ignore-gpu-blocklist
* #use-angle
	* According to the flag's description, using the OpenGL driver as the graphics backend may result in higher performance
	* D3D11 is used by default; D3D12 may improve performance if you are using Windows 10 1709 or newer.
                * Dịch 
                * Theo mô tả của cờ, việc sử dụng trình điều khiển OpenGL làm chương trình phụ trợ đồ họa có thể dẫn đến hiệu suất cao hơn
                * D3D11 được sử dụng theo mặc định; D3D12 có thể cải thiện hiệu suất nếu bạn đang sử dụng Windows 10 1709 hoặc mới hơn.
</p></details>

## Nguồn

<details><summary>Đây</summary><p>

*  `https://github.com/dreammjow/ChromiumHardening/blob/main/flags/flags.md`
</p></details>

<details><summary>Lí Do</summary><p>

* Lí Do Tui Copy Cái Này Để Test Thử Xem Gifhub như nào tiện tay nghịch tý 
</p></details>
