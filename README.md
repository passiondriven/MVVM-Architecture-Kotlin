## Kotlin MVVM Architecture

This is a simple application that display list/grid of available Google news. The purpose of this project to illustrate the usage of MVVM architecture design pattern that follow the best oractices of Object Oriented Design Patterns using the following technology stack.

 1. Architeture Design Pattern
 2. MVVM
 2. Dagger2 (Dependency Injection)
 3. Live Data, MediatorLiveData
 4. Room Database
 5. Retrofit
 6. Unit Testing (Espresso), Mockito (Coming soon)
 7. Repository Pattern
 8. AndroidX
 9. Glide
 10. NetworkBoundResource, NetworkAndDBBoundResource
 11. Google News API


## Architecture
<img alt="MVVM Architecture" height="600px" src="https://github.com/WaheedNazir/Kotlin-MVVM-Architecture/blob/master/screens/Architecture_design.jpg" />

### Dependencies used

      // Kotlin
    implementation "org.jetbrains.kotlin:kotlin-stdlib:$kotlinVersion"

    // Support Libraries
    implementation 'com.android.support:design:28.0.0'
    implementation 'androidx.appcompat:appcompat:1.1.0'
    implementation "com.android.support.constraint:constraint-layout:$constraintLayoutVersion"

    // Retrofit
    implementation "com.squareup.retrofit2:retrofit:$retrofitVersion"
    implementation "com.squareup.retrofit2:converter-gson:$retrofitVersion"
    implementation "com.squareup.okhttp3:logging-interceptor:$okHttpVersion"
    testImplementation "com.squareup.okhttp3:mockwebserver:$okHttpVersion"

    // Lifecycle (ViewModel + LiveData)
    implementation "androidx.lifecycle:lifecycle-extensions:$lifecycleVersion"
    kapt "androidx.lifecycle:lifecycle-compiler:$lifecycleVersion"
    implementation "android.arch.core:core-testing:$lifecycleVersion"

    // Room
    implementation "android.arch.persistence.room:runtime:$roomVersion"
    kapt "android.arch.persistence.room:compiler:$roomVersion"
    androidTestImplementation "android.arch.persistence.room:testing:$roomVersion"

    // Glide
    implementation "com.github.bumptech.glide:glide:$glideVersion"

    // Dagger core
    implementation "com.google.dagger:dagger:$dagger_version"
    kapt "com.google.dagger:dagger-compiler:$dagger_version"

    //Dagger Android
    implementation "com.google.dagger:dagger-android:$dagger_version"
    implementation "com.google.dagger:dagger-android-support:$dagger_version"
    kapt "com.google.dagger:dagger-android-processor:$dagger_version"

    //RxJava
    implementation 'io.reactivex.rxjava2:rxandroid:2.1.1'
    implementation "io.reactivex.rxjava2:rxjava:2.2.7"
    implementation 'com.jakewharton.retrofit:retrofit2-rxjava2-adapter:1.0.0'

    // Testing
    testImplementation "junit:junit:$jUnitVersion"
    androidTestImplementation("com.android.support.test.espresso:espresso-core:$espressoVersion", {
        exclude group: 'com.android.support', module: 'support-annotations'
    })

## Author
[Waheed Nazir](https://www.linkedin.com/in/waheed-nazir-36521579/ "Waheed Nazir (GreenProLogix)")

