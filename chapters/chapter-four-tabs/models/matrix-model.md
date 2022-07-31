# Matrix Model

### **Matrix Model**

![](https://lh6.googleusercontent.com/jlD2NDZw9BBkPOYUn9ccfgKQzCB1hzVhWR\_l15eo8446TupCMqsHqnk1Z5uYS\_D-VsC3d9tXg0QXB0oCoPTaze\_kP5QwWmiQYbCBV0yaKaxRJM2\_dvM1Y7GvWRzNcWmonFzxMD3F)

The direction can be defined as horizontal (the most common) or vertical. The ‘# Strings’ refers to the number of vertical columns of the matrix and the Lights/string refers to the number of nodes in each horizontal row. &#x20;

The starting location indicates where the matrix is connected to the controller (or where channel 1 of the matrix is).

![](https://lh3.googleusercontent.com/kaa-ZVjdFHQoaOG8PJ8ipke8Tma4Uqmn-0szajKunO\_-S0P6wKv5V\_pyOHDzov0dXDnblzOcUjHA\_gt0EYMpxYK9z62PRLH8oZoObCRn3UWq7iGdwKau628JA1s6RPkwgXG6ZkJ\_)

This is an example of a horizontal matrix used to define a P10 panel matrix. &#x20;

Each panel is (32 W x 16 H) pixels and the panel matrix is 8 panels in landscape.  The Start channel number is 11800.

For P10 panel matrices run off the BBB using the falcon player, , the matrix must always be defined as a horizontal matrix starting at the top left corner, irrespective of how the panels are physically  oriented.
