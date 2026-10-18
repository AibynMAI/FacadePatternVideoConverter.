Video Conversion System — Facade Pattern

Project Description

This project demonstrates the Facade structural design pattern using Java 17.

The system models a simplified video conversion workflow. The Facade coordinates input validation, source format detection, video data processing, audio processing, and conversion result creation.

The project is an educational simulation and does not perform actual video transcoding.

Technologies

* Java 17
* IntelliJ IDEA
* Facade Design Pattern

Main Classes

* Main — client application.
* VideoConversionFacade — simplified interface to the conversion workflow.
* InputValidator — validates user input.
* CodecFactory — identifies the source format.
* VideoFile — represents source video information.
* BitrateReader — models video data processing.
* AudioMixer — models audio processing.
* ConvertedFile — represents the conversion result.

How to Run

1. Open the project in IntelliJ IDEA.
2. Configure JDK 17.
3. Open Main.java.
4. Run the main() method.
5. Enter a source filename, such as movie.mp4.
6. Enter a supported target format, such as avi.

Supported target formats: mp4, avi, mkv, and mov.

Example

Input:

movie.mp4
avi

Output filename:

movie_converted.avi

Design Pattern

The Facade pattern provides a simplified interface to several subsystem classes.

The client calls VideoConversionFacade.convert() instead of coordinating subsystem operations directly.
