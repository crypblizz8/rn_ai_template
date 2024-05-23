# RN AI BoilerPlate

Quick BoilerPlate to make RN / Expo AI Apps

# Stack

AI Voice Stack
- Vapi
- Deepagram

Auth + DB

- Supabase
- Expo Apple Authentication

Style

- NativeWind

State

- Async Storage (due to supabase)
- (mmkv)
- (Zustand)

Navigation

- React Navigation

ENVS

- react dot env

# Prerequisites

## Supabase

- Create new project
- Get SUPABASE_URL and SUPABASE_ANON_KEY
- Then watch this YT tutorial (https://www.youtube.com/watch?v=6I2JEky20ME) You will need an Apple Dev Account
- On Dashboard --> Project Settings --> Authentication (https://supabase.com/dashboard/project/_/auth/providers)
- With `Authorized Client IDs`, add `iOS, host.exp.Exponent` because Expo needs authorization
- Ensure it is com.xxx.xxx not com.xxx.xxx.service

## ENVS

- Reference env.example
- Add into env


## Release Checklist for TestFlight
Prereq: Paid Apple Dev Account ($99)

Ensure your app name is not taken

- App Icons
- Splash Icons
- https://www.appicon.co/
- https://medium.com/how-tos/how-to-add-an-app-icon-and-a-launch-screen-to-your-xcode-project-7f29832d6f6c

Submitting (Expo)
- eas build --platform ios
   Use a new certificate for all
- eas submit -p ios
- Around 5 - 10 mins to buold
- increment version numbers: 
https://expo.fyi/bumping-ios-build-number 


Submitting (RN CLI if )
- XCode --> Product --> Archive
- Validate
- Distribute --> App Store

ENVS
- use EAS Secrets.

---

## Installation

1. Install dependencies

   ```bash
   npm install
   ```

2. Start the app

   ```bash
    npx expo start
   ```
