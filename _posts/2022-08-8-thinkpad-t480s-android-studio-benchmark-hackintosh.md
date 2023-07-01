---
title:  "Android Studio Perfomance Test on ThinkPad T480s ( Hackintosh )"
author: wakhid
date: 2022-08-8 12:32:00 -0500
categories: [Blogging, Hackintosh, Android Development, macOS]
tags: [ThinkPad, Laptop, Android Development, Hackintosh, macOS]
---


I am not an Android Developer. I conducted an Android Studio performance test on my ThinkPad T480s to contribute to the local ThinkPad community. Many members were interested in running Android Studio on their ThinkPad models.


## My ThinkPad T480s Specifications

- **Notebook model** : ThinkPad T480s
- **Operating System** : macOS Monterey 12.4 ( Hackintosh )
- **Android Studio version** : Chipmunk 2021.2.1 Patch 2 9 ( Java SDK 17 )
- **CPU Model** : i5 8350U 1.70 GHz ( Max Turbo 3.6 GHz )
- **RAM** : 20 GB
- **Storage** : NVME Intel SSDPEKKF512G8L capacity 500 GB
- **Test Results**: 3M 4s, 1m 55s, 1m 46s
- **Android Studio Benchmark Repository** : [https://github.com/yozhik/AndroidStudioBenchmark](https://github.com/yozhik/AndroidStudioBenchmark)

## 1st Build - BUILD SUCCESSFUL in 3m 4s
![1st Build](/images/wakhidcom_t480s_android_benchmark_1.png)

## 2nd Build - BUILD SUCCESSFUL in 1m 55s
![2nd Build](/images/wakhidcom_t480s_android_benchmark_2.png)

## 3rd Build - BUILD SUCCESSFUL in 1m 46s
![3rd Build](/images/wakhidcom_t480s_android_benchmark_3.png)

![3rd Build](/images/wakhidcom_t480s_android_benchmark_4.png)

---

## Sepecial Notes

- The maximum CPU temperature reached 95°C.
  The ThinkPad T480s series has known issues with CPU temperature, which have been addressed in Windows OS through a Lenovo driver update. In other operating systems, we may need to use undervoltage tools like https://github.com/sicreative/VoltageShift or https://github.com/erpalma/throttled. For better results in my test, I did not use any CPU tweaker software.

- The fan speed reached up to 4285 RPM.
  This is the maximum fan speed observed on the ThinkPad T480s.