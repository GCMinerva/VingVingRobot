## GCMinerva#24809 VingVingRobot Project ✨
###### VingVingRobot (วิ่งๆ โรบอท)  A path follower and robot management designed to revolutionize autonomous systhem in robotics including path follower movement , Servo controling , Camera color detecting
> [!CAUTION]
>  Beta version open to develope in school team no docs yet (Until testing done)
<img src="https://raw.githubusercontent.com/GCMinerva/VingVingRobot/refs/heads/main/VingVingRobot.png">

---

#### Install
```java
repositories {
    maven {
        url = uri("https://maven.vingving.jnx03.xyz")
    }
}

dependencies {
    implementation("com.vingvingrobot:core:0.0.1")
    implementation("com.vingvingrobot:ftc:0.0.1")
}
```

#### Sample Movement/path code
```java
VingPath path = new VingPath.Builder()
    .addWaypoint(new Waypoint.Builder(10, 10)
        .setSpeed(0.5)  // 50% speed
        .addAction(() -> servo.setPosition(0.8))
        .rotateTo(Math.toRadians(45))
        .stopAndWait(1.0)
        .build())
    .build();```
