# Checkpoint5-Approach shelf

## Introduction
<p>The goal of this project is to create a program that allows RB-1 robot to approach, detect, and attach a warehouse shelf.</p>

## Pre Approach
<p>The robot moves to the loading position. This requires two parameters- 1. obstacles: distance the robot will stop and 2. degrees: rotation the robot will turn to the shelf.</p>

    ros2 launch attach_shelf pre_approach.launch.xml obstacles:=0.3 degrees:=-90

[![pre_approach](https://res.cloudinary.com/marcomontalbano/image/upload/v1695271190/video_to_markdown/images/google-drive--1DgRmBbHia_gyzhEmwT6usviv4bih-cBS-c05b58ac6eb4c4700831b2b3070cd403.jpg)](https://drive.google.com/file/d/1DgRmBbHia_gyzhEmwT6usviv4bih-cBS/view?usp=sharing "pre_approach")

## Final Approach
<p>The robot will detect the shelf using laser intensity. If found, the robot will move toward the shelf and finally lift the shelf.</p>

    ros2 launch attach_shelf attach_to_shelf.launch.py obstacles:=0.3 degrees:=-90 final_approach:=True

[![final](https://res.cloudinary.com/marcomontalbano/image/upload/v1695301626/video_to_markdown/images/google-drive--15CeJtejYhWltBgUkOrjfqQTXfQ9NI5ia-c05b58ac6eb4c4700831b2b3070cd403.jpg)](https://drive.google.com/file/d/15CeJtejYhWltBgUkOrjfqQTXfQ9NI5ia/view?usp=sharing "final")
