#include <iostream>
#include <string>
using namespace std;

int main() {
    // ==========================================
    // 1. قسم المتغيرات والذاكرة (الصناديق السحرية)
    // ==========================================
    int distance_to_rock = 4;   // المسافة إلى الصخرة بالمتر
    bool scanner_active = true;     // حالة الحساس: يعمل بنجاح
    string robot_name = "Rover-X"; // اسم الروبوت الفضائي
cout << "=== " << robot_name << " Space OS Initialized ===" << endl;
 cout << ">> Scanner Status: " << (scanner_active ? "READY" : "OFF") << endl;
    cout << ">> Distance to closest obstacle: " << distance_to_rock << " meters." << endl;
    cout << "------------------------------------------" << endl;
    
    // ==========================================
    // 2. قسم اتخاذ القرار الذكي (عقل الروبوت)
    // ==========================================
    if (distance_to_rock <= 5) {
        cout << "🚨 DANGER DETECTED! Obstacle too close!" << endl;
        cout << ">> Executing protocol: Turning Right 90 Degrees... ✅" << endl;
    } else {
        cout << ">> Path Safe. Moving Forward! 🚀" << endl;
    }

    cout << "------------------------------------------" << endl;

    // ==========================================
    // 3. قسم مصنع التكرار وأتمتة جمع العينات (الـ For Loop)
    // ==========================================
    cout << "🚨 Arrived at safe zone. Starting Sample Collection..." << endl;
    
    for (int i = 1; i <= 5; i++) {
        cout << "Digging soil... [Sample #" << i << " Collected Successfully! 🚜]" << endl;
    }

    cout << "------------------------------------------" << endl;
    cout << "🏁 MISSION COMPLETE: All 10 samples are safe in the lab!" << endl;

    return 0;
}

