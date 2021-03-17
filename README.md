[![egui version: 0.10.0](https://img.shields.io/badge/egui%20version-0.10.0-orange)](https://docs.rs/egui/0.10.0/egui/index.html)
# epi_http 
epi::http implementation this enables all of egui platform have http download capability
## How to use
  ```rust
    #[cfg(feature="http")]
    let http=Arc::new( epi_http::EpiHttp{} );
    // some initialization code  here
    loop{
      let frame = FrameBuilder{
      info: IntegrationInfo,
      tex_allocator: &mut tex_allocator,
      repaint_signal: repaint_signal.clone(),
      output: &mut app_output,
      #[cfg(feature="http")]
      http: http.clone(),
      }
    }
  ```
##  Lack of support of  epi::http
  * [egui_winit_ash_vk_mem](https://crates.io/crates/egui_winit_ash_vk_mem)
  * [egui_wgpu_backend](https://crates.io/crates/egui_wgpu_backend)
  * [egui_vulkano_backend](https://crates.io/crates/egui_vulkano_backend)
  
