# Demo
To do POC
 curl \
    -F "status=2" \
    -F "notify=0" \
    -F "notes=$RELEASE_NOTES" \
    -F "notes_type=1" \
    -F "teams=Internal-Testers" \
    -F "ipa=@app/build/outputs/apk/$ENV_NAME/$APK_NAME" \
    -H "X-HockeyAppToken: $API_TOKEN" \
    https://rink.hockeyapp.net/api/2/apps/$2/app_versions/upload
