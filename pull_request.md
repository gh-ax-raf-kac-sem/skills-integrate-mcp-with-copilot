# Admin Mode Implementation

## Summary
This PR implements the admin authentication system requested in #5 to prevent students from removing each other from activities.

## Changes
- ✅ Added teacher login/logout with session token authentication
- ✅ Protected signup and unregister API endpoints
- ✅ Created login modal UI with user icon in header
- ✅ Added teachers.json file with sample credentials
- ✅ Hide delete buttons when not authenticated
- ✅ Disabled registration form for non-teachers

## Security
- Only authenticated teachers can register/unregister students
- Students can still view all activities and participants
- Session tokens validated on each protected API call

## Testing
Login with: `admin` / `admin123`

Closes #5