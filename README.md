# 🌾 Mobile App: FarmSpot

Farmspot is a mobile application designed to connect farmers directly with customers, bypassing intermediaries. This helps farmers earn more and allows customers to obtain higher-quality products. The app is developed using Android Studio, where we used programming languages such as Kotlin, Java, XML, among other technologies.

---

## 📱 What is Farmspot?

Farmspot is an innovative app that connects farmers directly with consumers, cutting out intermediaries. This ensures fair compensation for farmers and access to fresh, affordable produce for consumers. The platform simplifies transactions, making them efficient and user-friendly.

Farmspot acts as a marketplace where farmers list their products, and consumers can buy them at better prices. By removing supermarkets and other intermediaries, Farmspot reduces costs and improves quality. Users can create an account, search for products on a map, and discover nearby farms or specific items.

In summary, Farmspot aims to transform the agricultural supply chain by fostering direct interactions between farmers and consumers, promoting a more sustainable and fair marketplace.

---

## 🛠️ Description of the Main Features

### 3.1. User Interface (UI)
Farmspot features a modern and user-friendly interface. On launch, users are greeted with a loading screen displaying the app logo and a progress bar. After a brief delay, users are directed to the introduction screen where they can sign up or log in using Firestore Authentication. 

Authenticated users are taken to the main page, where they can browse and purchase products listed by other users. Each product has a dedicated page with detailed information and purchase options. If a user attempts to buy their own product, they receive a warning message. Purchased products are removed from the main page.

The app includes a map integration to display product locations using Google APIs. Users can also add new products through a form, including details such as name, description, location, category, price, and measurement unit.

Additional features include:
- 📜 **Purchase History**: Track past transactions.
- 👤 **Profile Management**: Manage account details and settings.
- 🆘 **Support Page**: Access contact information.

### 3.2. Persistent Storage
The app utilizes:
- **Firestore Database**: For storing product details, user information, and transaction records.
- **Firebase Storage**: For handling uploaded content associated with products.
- **Shared Preferences**: For storing local information like login status and user details.

### 3.3. Maps and Location
Farmspot's search functionality allows users to view product locations on a map. Geocoding converts location descriptions into geographical coordinates for accurate mapping. Users must grant location permissions for this feature to function.

### 3.4. Interaction with External Services
The app integrates Google Cloud services, including:
- **Maps APIs**: For displaying product locations.
- **Places APIs**: For searching points of interest.

---

## ⚙️ Description of the Secondary Features

### 4.1. Third-party Libraries
The app uses **Glide** for efficient image loading and management, simplifying the process of displaying product images.

### 4.2. Deployment on Physical Devices
The app was tested on an actual Android device by generating and installing the APK file to ensure functionality beyond the virtual environment.

### 4.3. Automated Tests
Automated UI tests were implemented to ensure functionality. Although there were challenges with Firebase testing libraries, database consistency was verified through various data operations and Firebase analytics.

### 4.4. Broadcast Receivers
Broadcast receivers handle delays in data updates, ensuring that the main page refreshes correctly after product uploads or sales, maintaining up-to-date information.

---

## 🛠️ Considerations to Execute the App in AVD

We strongly recommend using the **Pixel 2** as the emulated device when running the Android Virtual Device (AVD). All our mobile applications were developed with this device for optimal performance and compatibility. Additionally, we tested the app on a physical device, specifically a **Xiaomi Redmi**, with no additional changes required for smooth operation.

---

## 🚀 How to Execute the Mobile Application

To run the mobile application, you need to use Android Studio (an APK for Android devices is also provided). The .zip file includes all necessary files and instructions for setup, allowing users to easily deploy and test the application on their devices.

1. **Download the .zip file**: Ensure you have the .zip file containing all the necessary files.
2. **Extract the contents**: Unzip the file to a folder of your choice.
3. **Open Android Studio**: Launch Android Studio on your computer.
4. **Import the project**:
   - Go to `File` > `Open` in Android Studio.
   - Navigate to the folder where you extracted the .zip file and select the `build.gradle` file or the project folder.
5. **Sync the project**: Wait for Android Studio to sync the project. This may take a few moments as it downloads required dependencies.
6. **Set up an emulator or device**:
   - You can use an Android emulator or connect a physical device to your computer.
7. **Run the application**:
   - Click the `Run` button (the green triangle icon) at the top of Android Studio.
   - Select the emulator or connected device to deploy the application.

---
