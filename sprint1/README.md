# TuneTrackr
# Arjun Kalbag

### _TuneTrackr is a compact wearable music recognition device that instantly identifies songs with a single tap. Get song titles, artists, and album details once you conenct to your device. Lightweight, portable, and easy to use, it’s your go-to gadget for cataloging music on the fly._

## Goals

### MVP (Minimum Viable Product)
A functional device capable of initiating song recognition (potentially using the Shazam API) with the press of a button. Upon identification, the device will display essential information such as song title, artist, and album details.

### Goal
Develop a fully enclosed device with start/stop “searching” buttons (or a press-and-hold mechanism) and an integrated display for presenting song information.

### Extended Goal
Design a marketable casing with a refined user interface, featuring high-quality buttons for user interaction.

### Long-Term Objective
Implement an “add to Spotify” feature, allowing users to add recognized songs to their Spotify account with the press of a button, synced to the user's Spotify profile.

## Tasks

# Phase 1: Research, Planning, and Core Setup (1 Week)
- Task 1: Finalize the microcontroller (e.g., ESP32) and order necessary components (microphone, battery, mechanical switches).
- Task 2: Review song recognition API options (ACRCloud, AudioDB) and Spotify API setup.
- Task 3: Set up the development environment (e.g., Arduino IDE or PlatformIO) and install required libraries (Bluetooth, I2S, etc.).
# Phase 2: Prototyping Core Functions (2 Weeks)
_Week 2: Audio Recording and Bluetooth Transfer_
- Task 1: Set up the microphone and implement basic audio recording using I2S.
- Task 2: Implement file storage (either in memory or SD card).
- Task 3: Set up Bluetooth and transfer audio files to a mobile app or laptop.

_Week 3: Song Recognition Integration_

- Task 1: Integrate ACRCloud or AudioDB for song recognition (from the mobile app/laptop after receiving the file).
- Task 2: Code logic to handle recognized songs or display "No Music Found."
- Task 3: Test the full pipeline: recording audio → Bluetooth transfer → song recognition.
# Phase 3: Spotify and Dashboard Integration (2 Weeks)
_Week 4: Spotify API Integration_
- Task 1: Implement Spotify OAuth to authenticate and access your playlists.
- Task 2: Add recognized songs to a specific Spotify playlist.
- Task 3: Test song addition and ensure the playlist is updated correctly.

_Week 5: Dashboard Interface_

- Task 1: Build a basic dashboard (mobile app or web interface) to display recognized songs and manage the playlist.
- Task 2: Test real-time updating of recognized songs.
- Task 3: Debug any issues in song recognition, playlist updating, and dashboard display.
# Phase 4: Hardware and Power Design (2 Weeks)
_Week 6: Mechanical Keys and Power System_
- Task 1: Set up the mechanical key switches for the buttons (record, Bluetooth, power on/off).
- Task 2: Design the power system using a rechargeable LiPo battery and TP4056 charging module.
- Task 3: Test the power system, ensure smooth on/off switching, and verify battery charging.
# Phase 5: Case Design and Final Assembly (2 Weeks)
_Week 7: Case and Basic PCB Design (If Needed)_
- Task 1: Skip a custom PCB if time doesn’t permit; focus on basic wiring and setup of components.
- Task 2: Design a simple 3D-printed case for housing the components or use pre-made enclosures.
- Task 3: Assemble the components inside the case and test overall fit and functionality.

_Week 8: Final Testing and Debugging_ 

- Task 1: Conduct a full test of the system: audio recording, Bluetooth transfer, song recognition, Spotify playlist updating.
- Task 2: Optimize any delays in recognition, Bluetooth transfer, or battery performance.
- Task 3: Document the process and finalize the assembly.

<!-- ## Milestones
Break down your project into key tasks and milestones. Estimate the time required for each and the
order in which you'll complete them. Example structure:
| Task | Estimated Completion Time | Dependencies | Description |
|------|--------------------------|--------------|-------------|
| Task 1 | Week 1 | Materials | Initial connection between microcontrolelr, hardware, and computer. | 
| Task 2 | Week 2 | Task 1 | Connection to Music scanning functionality with working buttons. |
| Task 3 | Week 4 | Task 2 | Build a chasis/case for the device and get a working LED display. |
| Final Integration | Week 6 | Task 3 | Final touches (and maybe Spotify connection). | -->

## Challenges and Risks

_The biggest risk will be connecting the Shazam and/or Spotify APIs to the Microcontroller._

## Tools and Technologies

- Microcontroller (i.e. Particle Argon, Arduino, Rasberry PI Pico)
- Shazam/Music Recognition API
- Spotify API and OAuth
- C++ / (Micro) Python Coding Language
- Hardware
  - Buttons
  - PCB (Maybe Custom)
  - Key switches
    - Key Caps
  - Soldering gear
  - Breadboard for testing
  - Wires
  - Materials for case (maybe 3d printing fillament/laser cutter mat.)
  - LED display (maybe)
  - Memory chip
  - Recording Chip