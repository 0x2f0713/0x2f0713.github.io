---
layout: post
title:  "Upgrade RAM cho Orange Pi 3B v1.1"
date:   2025-09-28 10:00:00
categories: [sbc, orangepi]
tags: [story]
---

Đối với mỗi anh em IT, việc có một homelab/mini server ở nhà là điều thường thấy. Mình cùng vậy, cũng cần phải build 1 chú để self-host và tự chủ được những dịch vụ mà bớt phụ thuộc vào các Cloud.

Sau một thời gian sử dụng Android TV Box của tụi Amlogic chán chê, mình cần sang một dòng SoC mới hơn do nhu cầu của mình đã mở rộng ra, cụ thể là mình cần transcoding video bằng phần cứng thay vì CPU. Điều này Amlogic chưa làm được vì kernel chưa hỗ trợ tính năng này. Các nhà sản xuất SoC giá rẻ hiện nay như Allwinner, Amlogic,... thì thường sẽ viết mã nguồn đóng cho các tính năng trên. Tuy nhiên Rockchip thì public các source về hardware acceleration và chúng ta có thể dễ dàng build và xài với ffmpeg.

Chính vì vậy mình bắt đầu tìm các SBC dùng Rockchip và chủ yếu tìm đến dòng RK35xx do tính mới và trang bị thêm chút phần cứng hỗ trợ AI. Sau một thời gian thì mình cũng múc được một em Orange Pi 3B v1.1 phiên bản RAM 2GB với giá 7xxk từ một người pass 2nd.

Trong quá trình sử dụng, mình thấy 2GB RAM là chưa đủ nên mình suy nghĩ chuyện upgrade thêm. Bài viết này sẽ được update trong thời gian tới.

Những thông tin mình tìm kiếm được về chip RAM trên bo này.
- Mã chip: K4U6E3S4AB-MGCL https://semiconductor.samsung.com/dram/lpddr/lpddr4x/k4u6e3s4ab-mgcl/
- Density: 16 Gb
- Package: 200 FBGA
- Speed: 4266 Mbps
- Voltage: 1.8 / 1.1 / 0.6 V
- Organization: x32

Ngày 05/10/2025, mình có thêm một số thông tin là bản v2.1 của Orange Pi 3B 8GB sử dụng RAM Micron MT53E2G32D4DE-046 WT:C (https://www.micron.com/products/memory/dram-components/lpddr4/part-catalog/part-detail/mt53e2g32d4de-046-wt-c) và bản v1.1.1 8GB sử dụng chip SK Hynix H54G68CYRBX248N
