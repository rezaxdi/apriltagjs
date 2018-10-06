# AprilTagJS : A pure javascript implementation of AprilTag

*This implementation currently only supports 36H11 family and is under active developement so it is not recommended for production usage.*

## How to use ?

A working demo is available here : [demo](https://rezaxdi.github.io/apriltagjs/)

AprilTagJS depends on opencv.js, so first you need to include it in your project. (Latest nightly builds are available here : [opencv.js](https://docs.opencv.org/master/opencv.js)

```
let mat = cv.imread(imgSource);
detect(mat, (detections) => {
  detections.forEach((detection) => {
    console.log(detection.id);
    console.log(detection.hammingDistance);
    console.log(detection.points);
  });
});
```
