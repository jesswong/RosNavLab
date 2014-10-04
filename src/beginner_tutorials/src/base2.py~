#! /usr/bin/python
import time
import roslib
roslib.load_manifest('rospy')
roslib.load_manifest('geometry_msgs')
import rospy
from geometry_msgs.msg import *

if __name__ == "__main__":
	rospy.init_node('move_the_base', anonymous=True)
	
	topic_name = 'base_controller/command'
	pub = rospy.Publisher(topic_name, Twist)
	time.sleep(1)
	movement = Twist()
	movement.linear = Vector3(0.1, 0.0, 0.0)
	movement.angular = Vector3(0.0, 0.0, 0.0)
	
	"""
	start_time = rospy.get_rostime()
	while rospy.get_rostime() < start_time + rospy.Duration(30.0):
		pub.publish(movement)
		time.sleep(0.01)

	"""
	movement.linear = Vector3(0.0, 0.0, 0.0)
	movement.angular = Vector3(1.5, 1.5, 0.0)
	start_time = rospy.get_rostime()
	while rospy.get_rostime() < start_time + rospy.Duration(50.0):
		pub.publish(movement)
		time.sleep(0.01)
	"""


	movement.linear = Vector3(0.0, 0.1, 0.0)
	start_time = rospy.get_rostime()
	while rospy.get_rostime() < start_time + rospy.Duration(30.0):
		pub.publish(movement)
		time.sleep(0.01)

	movement.linear = Vector3(-0.1, 0.0, 0.0)
	start_time = rospy.get_rostime()
	while rospy.get_rostime() < start_time + rospy.Duration(30.0):
		pub.publish(movement)
		time.sleep(0.01)

	movement.linear = Vector3(0.0, -0.1, 0.0)
	start_time = rospy.get_rostime()
	while rospy.get_rostime() < start_time + rospy.Duration(50.0):
		pub.publish(movement)
		time.sleep(0.1)
	"""	

pub.publish(Twist())  # Stop
