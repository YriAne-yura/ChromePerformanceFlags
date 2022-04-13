
# Chrome Optimizations Lag Fix
Để Chỉnh Sửa Và Cài Đặt Vui Lòng Vào Đây `chrome://flags`
* Lưu ý : Trong Đây Đều Là Tiếng Anh Và Đã Có Bản Quyền Bên Dưới.
* My Channel: `https://www.youtube.com/channel/UC-FKTqZu2tO0-vgAM1S6dfw` ( Vietnamese ) 

## Tăng Hiệu Suất

<details><summary>Enabled</summary><p>

* #back-forward-cache - **Enabled force caching all pages (experimntal)**
	* Make sure you are using command line flags
* #enable-parallel-downloading
* #enable-skia-renderer
* #enable-quic
* #enable-throttle-display-none-and-visibility-hidden-cross-origin-iframes
* #enable-vulkan - Disabled, due to causing completely black web pages and making browsers laggy
	* This flag is enabled by default on some/most devices
	* If you don't experience the same problem, keep this flag default
* #enable-webassembly-lazy-compilation
	* This flag is placebo when JITLess mode and Strict Security mode in MS Edge are activated
* #overlay-strategies - **Occluded and unoccluded buffers (single-fullscreen,single-on-top,underlay)**
	* Use this flag for Skylake or newer
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
          Dịch 
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
