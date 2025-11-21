# CafeManagerPro - Kotlin Android App

Ứng dụng quản lý quán cà phê được xây dựng bằng Kotlin với kiến trúc MVVM.

## 🏗️ Kiến trúc

Dự án sử dụng **MVVM (Model-View-ViewModel)** architecture pattern:
- **Model**: Data classes và entities
- **View**: Activities và Fragments (chỉ xử lý UI)
- **ViewModel**: Quản lý UI-related data và business logic
- **Repository**: Tầng truy cập dữ liệu (Firebase, Room)

## 🛠️ Công nghệ sử dụng

- **Language**: Kotlin
- **Architecture**: MVVM
- **Dependency Injection**: Hilt
- **Database**: 
  - Firebase Realtime Database (remote)
  - Room Database (local cart)
- **UI**: Material Design Components
- **Image Loading**: Glide
- **Coroutines & Flow**: Reactive programming
- **Payment**: VNPay, Blockchain (Ethereum Sepolia)

## 📋 Yêu cầu

- Android Studio Hedgehog | 2023.1.1 trở lên
- JDK 17
- Android SDK 23 (minSdk) - 34 (targetSdk)
- Gradle 8.0+



## 📁 Cấu trúc thư mục

```
app/src/main/java/com/pro/shopfee/
├── activity/          # Activities
├── fragment/          # Fragments
├── viewmodel/         # ViewModels (MVVM)
├── repository/        # Repository layer
├── model/             # Data models
├── adapter/           # RecyclerView adapters
├── database/          # Room database
├── di/                # Hilt dependency injection modules
├── utils/             # Utility classes
└── prefs/             # SharedPreferences/DataStore
```


## 📝 Tính năng

- ✅ Đăng nhập/Đăng ký (Firebase Auth)
- ✅ Quản lý sản phẩm (Drinks, Categories)
- ✅ Giỏ hàng (Room Database)
- ✅ Đặt hàng với nhiều phương thức thanh toán:
  - VN Pay 
  - Blockchain (Ethereum Sepolia) - quy đổi tỉ giá theo thời gian thực
- ✅ Quản lý đơn hàng
- ✅ Đánh giá sản phẩm
- ✅ Voucher/Discount
- ✅ Tính phí vận chuyển theo khoảng cách
- ✅ Quản lý địa chỉ
- ✅ Hệ thống hạng thành viên

## 👥 Phân quyền

- **User**: Xem sản phẩm, đặt hàng, quản lý đơn hàng
- **Admin**: Quản lý sản phẩm, đơn hàng, voucher, xem feedback
  
