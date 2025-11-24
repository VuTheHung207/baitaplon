# baitaplon
<!DOCTYPE html>
<html lang="vi" style="scroll-behavior: smooth;">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SmartFarm - Công Nghệ Tưới Tiêu Thông Minh</title>
    <!-- Tải Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Tải Font Inter -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@100..900&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f7f9fb; /* Nền nhẹ nhàng */
        }
        .section-padding {
            padding: 5rem 1rem;
        }
        .card {
            box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s ease-in-out;
        }
        .card:hover {
            transform: translateY(-5px);
        }
        /* Custom scrollbar for demo purposes, if supported */
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-thumb {
            background: #10b981;
            border-radius: 4px;
        }
        /* Style cho nút "Đặt hàng ngay" */
        .primary-btn {
            background-image: linear-gradient(to right, #10b981 0%, #059669 100%);
            transition: all 0.3s ease;
        }
        .primary-btn:hover {
            opacity: 0.9;
            transform: scale(1.02);
        }
    </style>
</head>
<body>

    <!-- Thanh Điều Hướng (Navigation Bar) -->
    <nav id="navbar" class="sticky top-0 z-50 bg-white shadow-lg">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-16">
                <!-- Logo -->
                <a href="#trang-chu" class="flex-shrink-0 text-2xl font-extrabold text-[#10b981] tracking-tight">
                    SmartFarm
                </a>

                <!-- Desktop Menu -->
                <div class="hidden sm:ml-6 sm:flex sm:space-x-8">
                    <a href="#trang-chu" class="text-gray-900 hover:text-[#059669] px-3 py-2 rounded-md text-sm font-medium transition duration-150">Trang Chủ</a>
                    <a href="#san-pham" class="text-gray-900 hover:text-[#059669] px-3 py-2 rounded-md text-sm font-medium transition duration-150">Sản Phẩm</a>
                    <a href="#case-study" class="text-gray-900 hover:text-[#059669] px-3 py-2 rounded-md text-sm font-medium transition duration-150">Case Study</a>
                    <a href="#" class="primary-btn text-white px-4 py-2 rounded-full text-sm font-semibold ml-4 shadow-lg flex items-center">
                        Tư Vấn Ngay
                    </a>
                </div>

                <!-- Mobile Menu Button (Hamburger) -->
                <div class="sm:hidden flex items-center">
                    <button id="mobile-menu-button" class="inline-flex items-center justify-center p-2 rounded-md text-gray-400 hover:text-gray-500 hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-inset focus:ring-[#10b981]">
                        <svg class="h-6 w-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7" />
                        </svg>
                    </button>
                </div>
            </div>
        </div>

        <!-- Mobile Menu (Hidden by default) -->
        <div id="mobile-menu" class="hidden sm:hidden">
            <div class="px-2 pt-2 pb-3 space-y-1">
                <a href="#trang-chu" class="text-gray-900 hover:bg-gray-50 block px-3 py-2 rounded-md text-base font-medium">Trang Chủ</a>
                <a href="#san-pham" class="text-gray-900 hover:bg-gray-50 block px-3 py-2 rounded-md text-base font-medium">Sản Phẩm</a>
                <a href="#case-study" class="text-gray-900 hover:bg-gray-50 block px-3 py-2 rounded-md text-base font-medium">Case Study</a>
                <a href="#" class="primary-btn text-white block px-3 py-2 rounded-md text-base font-medium text-center mt-2 mx-2">Tư Vấn Ngay</a>
            </div>
        </div>
    </nav>

    <!-- TRANG CHỦ -->
    <section id="trang-chu" class="section-padding bg-white">
        <div class="max-w-7xl mx-auto">
            <!-- 1. Sản phẩm công nghệ & Demo Video -->
            <div class="grid md:grid-cols-2 gap-12 items-center">
                <!-- Giới thiệu Sản phẩm -->
                <div>
                    <span class="inline-block bg-[#e0f2f1] text-[#047857] text-sm font-medium px-4 py-1 rounded-full mb-3">#1 Công Nghệ Nông Nghiệp</span>
                    <h1 class="text-5xl md:text-6xl font-extrabold text-gray-900 leading-tight mb-6">
                        Tưới Tiêu Thông Minh <span class="text-[#10b981]">Tối Ưu</span> Hiệu Quả
                    </h1>
                    <p class="text-xl text-gray-600 mb-8">
                        SmartFarm mang đến giải pháp tưới tự động dựa trên AI, phân tích dữ liệu thời tiết và độ ẩm đất để cung cấp lượng nước chính xác, tiết kiệm 50% nước và tăng năng suất cây trồng.
                    </p>
                    <div class="flex space-x-4">
                        <a href="#san-pham" class="primary-btn text-white px-8 py-3 rounded-xl text-lg font-semibold shadow-xl hover:shadow-2xl">
                            Khám Phá Sản Phẩm
                        </a>
                        <a href="#demo-video" class="text-gray-800 border-2 border-gray-300 px-8 py-3 rounded-xl text-lg font-semibold hover:bg-gray-100 transition duration-150 flex items-center">
                            <svg class="w-5 h-5 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M14.752 11.168l-3.197-2.132A1 1 0 0010 9.87v4.26a1 1 0 001.555.832l3.197-2.132a1 1 0 000-1.664z"></path><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 12a9 9 0 11-18 0 9 9 0 0118 0z"></path></svg>
                            Xem Demo
                        </a>
                    </div>
                </div>

                <!-- Hình ảnh/Video Placeholder -->
                <div class="relative aspect-video rounded-lg overflow-hidden shadow-2xl">
                    <!-- Iframe nhúng video Youtube -->
                    <iframe 
                        class="w-full h-full absolute inset-0"
                        src="https://www.youtube.com/embed/4QbtJCvz9SA" 
                        title="YouTube video player" 
                        frameborder="0" 
                        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
                        allowfullscreen>
                    </iframe>
                </div>

            <!-- 2. Ưu đãi mua hàng -->
          
           </div>
        </div>
    </section>
                <!-- Ưu Đãi Đặc Biệt Cho Khách Hàng Mới -->
    <section id="dai-ngo" class="w-full bg-gray-50 py-20">
    <div class="w-full px-6">
        <h2 class="text-4xl font-bold text-center text-gray-900 mb-10">Ưu Đãi Đặc Biệt Cho Khách Hàng Mới</h2>

        <div class="grid md:grid-cols-3 gap-8 max-w-7xl mx-auto">
            <!-- Ưu đãi 1 -->
            <div class="card p-6 bg-white rounded-xl border-t-4 border-[#34d399]">
                <h3 class="text-2xl font-semibold text-gray-800 mb-3">Miễn Phí Lắp Đặt</h3>
                <p class="text-gray-600 mb-4">Áp dụng cho mọi đơn hàng hệ thống tưới tiêu trọn gói trên 2 hecta.</p>
                <div class="text-4xl font-extrabold text-[#10b981]">100% OFF</div>
            </div>

            <!-- Ưu đãi 2 -->
            <div class="card p-6 bg-white rounded-xl border-t-4 border-[#34d399]">
                <h3 class="text-2xl font-semibold text-gray-800 mb-3">Tặng Cảm Biến Độ Ẩm</h3>
                <p class="text-gray-600 mb-4">Tặng kèm 03 cảm biến đất tiên tiến khi mua bộ điều khiển trung tâm.</p>
                <div class="text-4xl font-extrabold text-[#10b981] flex items-end">
                    03 <span class="text-xl ml-2 text-gray-500">Thiết Bị</span>
                </div>
            </div>

            <!-- Ưu đãi 3 -->
            <div class="card p-6 bg-white rounded-xl border-t-4 border-[#34d399]">
                <h3 class="text-2xl font-semibold text-gray-800 mb-3">Giảm Giá Phần Mềm</h3>
                <p class="text-gray-600 mb-4">Giảm 50% phí duy trì ứng dụng quản lý trong năm đầu tiên sử dụng.</p>
                <div class="text-4xl font-extrabold text-[#10b981]">50% OFF</div>
            </div>
        </div>
    </div>
</section>

    <!-- TRANG SẢN PHẨM -->
    <section id="san-pham" class="section-padding bg-[#f0fdf4]">
        <div class="max-w-7xl mx-auto">
            <h2 class="text-4xl font-bold text-center text-gray-900 mb-16">Chi Tiết Giải Pháp SmartFarm</h2>

            <!-- Đặc tính kỹ thuật -->
            <div class="mb-16">
                <h3 class="text-3xl font-semibold text-[#065f46] mb-8 border-b-2 border-[#a7f3d0] pb-2">1. Đặc Tính Kỹ Thuật</h3>
                <div class="grid md:grid-cols-3 gap-8">
                    <div class="card p-6 bg-white rounded-xl">
                        <div class="text-[#10b981] mb-3">
                            <svg class="w-8 h-8" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9.75 17L9 20l-1 1h8l-1-1v-3"></path><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 2v20"></path><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 4.75a.75.75 0 00-1.5 0v1.5a.75.75 0 001.5 0v-1.5zM12 7.75a.75.75 0 00-1.5 0v1.5a.75.75 0 001.5 0v-1.5zM12 10.75a.75.75 0 00-1.5 0v1.5a.75.75 0 001.5 0v-1.5zM12 13.75a.75.75 0 00-1.5 0v1.5a.75.75 0 001.5 0v-1.5z"></path><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 19H7a4 4 0 01-4-4V7a4 4 0 014-4h10a4 4 0 014 4v8a4 4 0 01-4 4z"></path></svg>
                        </div>
                        <h4 class="text-xl font-semibold mb-2">Bộ Điều Khiển Trung Tâm (Hub)</h4>
                        <p class="text-gray-600">Chip AI xử lý 10,000 dữ liệu/giây. Phạm vi kết nối LoRaWAN lên đến 5km. Pin dự phòng 48 giờ.</p>
                    </div>
                    <div class="card p-6 bg-white rounded-xl">
                        <div class="text-[#10b981] mb-3">
                            <svg class="w-8 h-8" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z"></path></svg>
                        </div>
                        <h4 class="text-xl font-semibold mb-2">Cảm Biến Đất & Thời Tiết</h4>
                        <p class="text-gray-600">Đo độ ẩm, nhiệt độ, pH đất và lượng mưa tức thời. Độ chính xác 99.8%. Chống nước IP68.</p>
                    </div>
                    <div class="card p-6 bg-white rounded-xl">
                        <div class="text-[#10b981] mb-3">
                            <svg class="w-8 h-8" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8c-2.003 0-3.953.535-5.6 1.545M12 8l.261-.132A6.84 6.84 0 0012 8z"></path><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8c2.003 0 3.953.535 5.6 1.545M12 8l-.261-.132A6.84 6.84 0 0012 8z"></path><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 12h-6"></path><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 15h-6"></path><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 21v-2a4 4 0 00-4-4H9a4 4 0 00-4 4v2"></path><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M10 7L8 4"></path><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M14 7L16 4"></path></svg>
                        </div>
                        <h4 class="text-xl font-semibold mb-2">Giao Thức Mở Rộng</h4>
                        <p class="text-gray-600">Tương thích với các loại van điện từ và bơm phổ biến. Hỗ trợ Modbus, Zigbee và Wi-Fi.</p>
                    </div>
                </div>
            </div>

            <!-- Quy trình Lắp đặt -->
            <div class="mb-16">
                <h3 class="text-3xl font-semibold text-[#065f46] mb-8 border-b-2 border-[#a7f3d0] pb-2">2. Quy Trình Lắp Đặt Đơn Giản</h3>
                <div class="grid md:grid-cols-4 gap-6 text-center">
                    <div class="card p-6 bg-white rounded-xl">
                        <div class="w-12 h-12 flex items-center justify-center mx-auto rounded-full bg-[#ecfdf5] text-[#065f46] text-xl font-bold mb-3">1</div>
                        <h4 class="font-bold mb-2">Khảo Sát</h4>
                        <p class="text-sm text-gray-600">Đội ngũ kỹ thuật đánh giá địa hình và nhu cầu cây trồng.</p>
                    </div>
                    <div class="card p-6 bg-white rounded-xl">
                        <div class="w-12 h-12 flex items-center justify-center mx-auto rounded-full bg-[#ecfdf5] text-[#065f46] text-xl font-bold mb-3">2</div>
                        <h4 class="font-bold mb-2">Lắp Đặt Hub</h4>
                        <p class="text-sm text-gray-600">Cài đặt Bộ Điều Khiển Trung Tâm và kết nối nguồn điện.</p>
                    </div>
                    <div class="card p-6 bg-white rounded-xl">
                        <div class="w-12 h-12 flex items-center justify-center mx-auto rounded-full bg-[#ecfdf5] text-[#065f46] text-xl font-bold mb-3">3</div>
                        <h4 class="font-bold mb-2">Cài Cảm Biến</h4>
                        <p class="text-sm text-gray-600">Chôn cảm biến độ ẩm tại các điểm đại diện trong khu vực canh tác.</p>
                    </div>
                    <div class="card p-6 bg-white rounded-xl">
                        <div class="w-12 h-12 flex items-center justify-center mx-auto rounded-full bg-[#ecfdf5] text-[#065f46] text-xl font-bold mb-3">4</div>
                        <h4 class="font-bold mb-2">Vận Hành App</h4>
                        <p class="text-sm text-gray-600">Thiết lập ngưỡng tưới và kịch bản tự động trên ứng dụng.</p>
                    </div>
                </div>
            </div>

            <!-- Tích hợp App -->
            <div>
                <h3 class="text-3xl font-semibold text-[#065f46] mb-8 border-b-2 border-[#a7f3d0] pb-2">3. Ứng Dụng Quản Lý (Mobile App)</h3>
                <div class="grid md:grid-cols-2 gap-12 items-center">
                    <div class="bg-[#d1fae5] rounded-3xl p-8 flex items-center justify-center h-full min-h-64">
                         <img 
                            src="99.jpg" 
                            alt="SmartFarm App"
                            class="rounded-xl max-h-80 object-contain" >
                    </div>
                    <ul class="space-y-6">
                        <li class="flex items-start">
                            <span class="text-[#10b981] mr-3 mt-1 flex-shrink-0">
                                <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd"></path></svg>
                            </span>
                            <div>
                                <h4 class="font-semibold text-lg text-gray-900">Giám Sát Thời Gian Thực:</h4>
                                <p class="text-gray-600">Theo dõi độ ẩm, nhiệt độ, và trạng thái van tưới mọi lúc, mọi nơi.</p>
                            </div>
                        </li>
                        <li class="flex items-start">
                            <span class="text-[#10b981] mr-3 mt-1 flex-shrink-0">
                                <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd"></path></svg>
                            </span>
                            <div>
                                <h4 class="font-semibold text-lg text-gray-900">Lập Lịch Tưới Thông Minh:</h4>
                                <p class="text-gray-600">Thiết lập kịch bản tưới tự động dựa trên dự báo thời tiết và dữ liệu đất đai.</p>
                            </div>
                        </li>
                        <li class="flex items-start">
                            <span class="text-[#10b981] mr-3 mt-1 flex-shrink-0">
                                <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd"></path></svg>
                            </span>
                            <div>
                                <h4 class="font-semibold text-lg text-gray-900">Báo Cáo Chi Tiết:</h4>
                                <p class="text-gray-600">Xuất báo cáo về lượng nước tiêu thụ, chi phí điện, và hiệu suất tưới hàng tuần/tháng.</p>
                            </div>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- TRANG CASE STUDY -->
    <section id="case-study" class="section-padding bg-white">
        <div class="max-w-7xl mx-auto">
            <h2 class="text-4xl font-bold text-center text-gray-900 mb-16">Hiệu Quả Thực Tế Từ Khách Hàng</h2>

            <!-- Ví dụ Thực tế & Dữ liệu Tiết kiệm Nước -->
            <div class="grid md:grid-cols-2 gap-12 items-center mb-20">
                <!-- Ví dụ Thực Tế -->
                <div>
                    <h3 class="text-3xl font-semibold text-[#065f46] mb-4">Case Study: Vườn Thanh Long Bến Tre</h3>
                    <p class="text-gray-600 mb-6">
                        Trước đây, vườn Thanh Long rộng 5 hecta của ông Nguyễn Văn A tiêu thụ trung bình 500m³ nước/tuần. Sau khi lắp đặt SmartFarm, hệ thống đã điều chỉnh lịch tưới theo mùa và tiết kiệm được một lượng nước đáng kể, đồng thời cây cho năng suất cao hơn 15%.
                    </p>
                    <a href="#" class="text-[#059669] font-medium hover:underline">Xem toàn bộ báo cáo chi tiết &rarr;</a>
                </div>
                <!-- Dữ liệu Tiết kiệm Nước -->
                <div class="bg-[#f0fdf4] p-8 rounded-xl card">
                    <h4 class="text-2xl font-bold text-gray-800 mb-4">Dữ Liệu Tiết Kiệm Nước Trung Bình</h4>
                    <div class="grid grid-cols-3 gap-4 text-center">
                        <div class="p-4 bg-white rounded-lg shadow-md">
                            <p class="text-4xl font-extrabold text-[#10b981]">50%</p>
                            <p class="text-sm text-gray-500">Tiết kiệm Nước</p>
                        </div>
                        <div class="p-4 bg-white rounded-lg shadow-md">
                            <p class="text-4xl font-extrabold text-[#10b981]">25%</p>
                            <p class="text-sm text-gray-500">Giảm Chi phí Điện</p>
                        </div>
                        <div class="p-4 bg-white rounded-lg shadow-md">
                            <p class="text-4xl font-extrabold text-[#10b981]">15%</p>
                            <p class="text-sm text-gray-500">Tăng Năng Suất</p>
                        </div>
                    </div>
                    <p class="text-sm text-gray-500 mt-4 italic">Dữ liệu tổng hợp từ 20 trang trại đã triển khai trong 6 tháng.</p>
                </div>
            </div>

            <!-- Testimonial (Lời chứng thực) -->
            <div>
                <h3 class="text-3xl font-semibold text-[#065f46] mb-8 border-b-2 border-[#a7f3d0] pb-2">2. Đánh Giá Từ Khách Hàng</h3>
                <div class="grid md:grid-cols-3 gap-8">
                    <!-- Đánh giá 1 -->
                    <div class="card p-6 bg-[#f7f9fb] rounded-xl border-l-4 border-[#10b981] shadow-lg">
                        <p class="text-lg italic text-gray-700 mb-4">"Hệ thống SmartFarm thực sự là bước đột phá. Tôi không cần lo lắng về việc tưới tiêu nữa, mọi thứ đều tự động và chính xác. Năng suất cà phê tăng rõ rệt!"</p>
                        <div class="flex items-center">
                            <div class="w-10 h-10 bg-gray-300 rounded-full flex items-center justify-center text-sm font-bold text-gray-600 mr-3">AV</div>
                            <div>
                                <p class="font-semibold text-gray-900">Anh Văn</p>
                                <p class="text-sm text-gray-500">Chủ trang trại Cà phê Đà Lạt</p>
                            </div>
                        </div>
                    </div>
                    <!-- Đánh giá 2 -->
                    <div class="card p-6 bg-[#f7f9fb] rounded-xl border-l-4 border-[#10b981] shadow-lg">
                        <p class="text-lg italic text-gray-700 mb-4">"Việc tiết kiệm nước là ưu tiên hàng đầu của chúng tôi. Với SmartFarm, chúng tôi giảm được 55% lượng nước so với phương pháp truyền thống. Quá tuyệt vời!"</p>
                        <div class="flex items-center">
                            <div class="w-10 h-10 bg-gray-300 rounded-full flex items-center justify-center text-sm font-bold text-gray-600 mr-3">LT</div>
                            <div>
                                <p class="font-semibold text-gray-900">Chị Lan</p>
                                <p class="text-sm text-gray-500">Quản lý khu nông nghiệp hữu cơ</p>
                            </div>
                        </div>
                    </div>
                    <!-- Đánh giá 3 -->
                    <div class="card p-6 bg-[#f7f9fb] rounded-xl border-l-4 border-[#10b981] shadow-lg">
                        <p class="text-lg italic text-gray-700 mb-4">"Lắp đặt dễ dàng, đội ngũ hỗ trợ tận tình. Ứng dụng quản lý rất trực quan, ngay cả người lớn tuổi như tôi cũng sử dụng thành thạo."</p>
                        <div class="flex items-center">
                            <div class="w-10 h-10 bg-gray-300 rounded-full flex items-center justify-center text-sm font-bold text-gray-600 mr-3">TA</div>
                            <div>
                                <p class="font-semibold text-gray-900">Ông Tuấn</p>
                                <p class="text-sm text-gray-500">Nông dân trồng lúa công nghệ cao</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-800 text-white py-12">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-2 md:grid-cols-4 gap-8">
                <!-- Cột 1: Logo & Slogan -->
                <div>
                    <h3 class="text-2xl font-extrabold text-[#10b981] mb-4">SmartFarm</h3>
                    <p class="text-gray-400 text-sm">Tối ưu hóa nông nghiệp, bảo vệ tài nguyên.</p>
                </div>
                <!-- Cột 2: Liên kết nhanh -->
                <div>
                    <h4 class="font-semibold text-lg mb-4">Liên Kết</h4>
                    <ul class="space-y-2">
                        <li><a href="#trang-chu" class="text-gray-400 hover:text-[#10b981] transition duration-150 text-sm">Trang Chủ</a></li>
                        <li><a href="#san-pham" class="text-gray-400 hover:text-[#10b981] transition duration-150 text-sm">Sản Phẩm</a></li>
                        <li><a href="#case-study" class="text-gray-400 hover:text-[#10b981] transition duration-150 text-sm">Case Study</a></li>
                    </ul>
                </div>
                <!-- Cột 3: Thông tin liên hệ -->
                <div>
                    <h4 class="font-semibold text-lg mb-4">Hỗ Trợ</h4>
                    <ul class="space-y-2 text-sm">
                        <li class="text-gray-400">Hotline: 0397684806</li>
                        <li class="text-gray-400">Email: vuthehung241007@gmail.com</li>
                        <li class="text-gray-400">Địa chỉ:  Hà Nội</li>
                    </ul>
                </div>
                <!-- Cột 4: Đăng ký nhận tin -->
                <div>
                    <h4 class="font-semibold text-lg mb-4">Nhận Tin Tức</h4>
                    <p class="text-gray-400 text-sm mb-3">Nhận các ưu đãi mới nhất qua email.</p>
                    <div class="flex">
                        <input type="email" placeholder="Email của bạn" class="p-2 rounded-l-lg text-gray-900 focus:outline-none w-full">
                        <button class="primary-btn px-4 rounded-r-lg text-sm font-semibold">Gửi</button>
                    </div>
                </div>
            </div>
            <div class="mt-10 pt-6 border-t border-gray-700 text-center text-gray-500 text-sm">
                &copy; 2024 SmartFarm. All rights reserved.
            </div>
        </div>
    </footer>

    <!-- JavaScript for Mobile Menu & Scroll Smoothing -->
    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const mobileMenuButton = document.getElementById('mobile-menu-button');
            const mobileMenu = document.getElementById('mobile-menu');

            // 1. Toggle mobile menu visibility
            mobileMenuButton.addEventListener('click', () => {
                mobileMenu.classList.toggle('hidden');
            });

            // 2. Hide mobile menu after clicking a link (for smooth navigation)
            const mobileLinks = mobileMenu.querySelectorAll('a');
            mobileLinks.forEach(link => {
                link.addEventListener('click', () => {
                    mobileMenu.classList.add('hidden');
                });
            });

            // Note: HTML's 'scroll-behavior: smooth' handles the smooth scrolling effect itself.
        });
    </script>
</body>
</html>
