<html>
  <body>
    <h1>Drone Square Action</h1>
    <p>
      This code defines a ROS action server that controls a drone to perform a square. The square consists of moving forward for a specified amount of time, then turning for a specified amount of time, and repeating this process four times. The total time it takes for the drone to perform the square is calculated and returned as the result of the action.
    </p>
    <h2>Dependencies</h2>
    <ul>
      <li>ROS</li>
      <li>actionlib</li>
      <li>drone_sq_server</li>
      <li>geometry_msgs</li>
      <li>ros</li>
      <li>std_msgs</li>
    </ul>
    <h2>Code Explanation</h2>
    <p>
      The code defines a <code>SquareAction</code> class that inherits from <code>actionlib::SimpleActionServer</code>. The constructor of this class initializes the action server and sets up publishers for the <code>/cmd_vel</code>, <code>/drone/takeoff</code>, and <code>/drone/land</code> topics. The <code>executeCB()</code> method is called when the action server receives a goal from a client. This method controls the drone to perform the square and returns the total time it took to complete the square as the result of the action.
    </p>
    <h2>Functions</h2>
    <ul>
      <li><code>takeoff_drone()</code>: Controls the drone to take off</li>
      <li><code>stop_drone()</code>: Stops the drone's movement</li>
      <li><code>move_forward_drone(int side_secs)</code>: Controls the drone to move forward for a specified amount of time</li>
      <li><code>turn_drone(int turn_secs)</code>: Controls the drone to turn for a specified amount of time</li>
      <li><code>land_drone()</code>: Controls the drone to land</li>
    </ul>
  </body>
</html>
