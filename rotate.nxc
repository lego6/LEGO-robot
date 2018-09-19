sub rotate(int, int, int);
sub rotate_primitive(int, int, int);

task main() {
    // 1 ..... find shortest distance to wall

    // 2 ..... approach wall 0-30cm

    // 3 ..... rotate 90 degrees

    rotate(50, 90, 1);

    wait(5000);

    rotate_primitive(50, 50, 1);

    wait(5000);

    rotate(50, 90, 4);

    wait(5000);

    rotate_primitive(50, 50, 4);    


    // 4 ..... drive 2.5m

    // 5 ..... drop mail
}

sub rotate_primitive(int leftWheel, int rightWheel, int mode) {
    if (mode == 3 || mode == 4) {
        OnFwd(OUT_B, leftWheel);
        OnRev(OUT_C, rightWheel);
        Wait(1500);
    }
    // oliver function
    if (mode == 1 || mode == 3) {
        OnFwd(OUT_B, leftWheel);
        OnRev(OUT_C, rightWheel);
        Wait(750);
    } else {
        OnRev(OUT_B, leftWheel);
        OnFwd(OUT_C, rightWheel);
        Wait(750);
    }
}

sub rotate(int speed, int degrees, int mode) {
    if (mode == 3 || mode == 4) {
        RotateMotorEx(OUT_BC, speed, degrees * 2, 0, true, true);
    }
    // oliver function
    if (mode == 1 || mode == 3) {
        RotateMotorEx(OUT_BC, speed, degrees, 0, true, true);
    } else {
        RotateMotorEx(OUT_BC, speed, degrees, 0, true, true);
    }
}
