
# Event-Notifications
- When life-cycle transitions an object, u can get a notification
- When life-cycle expires an object, u can get a notification
- This can help u change dynamodb table indexes due to expiry notification
- Companies like CNN can store data in Deep Archive that they do not need. Let's say they want to broadcast a news and
  show some old video. What they do is they make an expedited request on the video file and get a notification when its 
  in S3-Standard which will be available for instant access.