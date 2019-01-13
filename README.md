# julia-folder-combiner
It takes two folders containing an arbitrary number of files and combines them with the files renamed sequentially. Good for disparate collections of images or a whole mess of audio samples.

## What it do

Obviously incomplete, but essentially you either run it in a directory containing the folders you want to process and it combines **all** of them, or you can specify which folders to combine with commandline arguments.

Input should look like:

**folder1/**

  thing1.jpg

  thing2.jpg
  
  ...
  
  thingn.jpg
  
*folder2/*
  
  whatevs1.jpg
  
  whatevs59.jpg
  
  yarp55.jpg
  
And then the output will be:

**output/**
  
  001.jpg
  
  002.jpg
  
  ...

Works with globbing on Linux. Note that it uses default sorting for determining the output filenames and it maintains extensions.

## What it could

It would be great if the output filenames were more informative, like they contained the date the original file was created or for mp3s it rewrote the metadata to change the track number to make a compilation or something.