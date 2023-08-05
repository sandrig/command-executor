# Command executor

A command-line utility to convert video files from .mov format to .mp4 format.

Step-by-step description:

1. Clone this repository:

- Create a folder for the project and navigate to it in the command line.
- Clone the repository using the command: git clone <repository URL>. Replace <repository URL> with the URL of the repository containing the source code of the utility.

2. Install FFmpeg:

- Make sure you have Homebrew package manager installed (for macOS).
- Install FFmpeg using the command: brew install ffmpeg.

3. Install dependencies:

- Ensure that you have Node.js and npm (or pnpm) package manager installed.
- Install pnpm if you don't have it yet, using the command: npm install -g pnpm.
- Then, install project dependencies by running: pnpm install.

4. Copy the .mov file:

- Place the .mov file you want to convert to .mp4 in the root directory of the application (where the app.js file is located).

5. Compile TypeScript:

- Ensure that you have TypeScript installed globally (if not done previously) using the command: npm install typescript -g.
- Compile the TypeScript files by executing: tsc.

6. Execute the utility:

- Run the command-line utility to convert .mov to .mp4 using: node ./dist/app.js <parameters>.
- Replace <parameters> with the necessary conversion parameters:
  - **width**: Video width (optional).
  - **height**: Video height (optional).
  - **path to file**: Path to the .mov file you want to convert.
  - **name**: Name for the resulting .mp4 file (optional).

An example command to execute the utility could be:

```bash
node ./dist/app.js --width 1920 --height 1080 --path-to-file input.mov --name output.mp4
```

The utility will convert the input.mov file to .mp4 format with the specified parameters (width and height) and save it as output.mp4 in the same directory as the utility.
