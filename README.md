- š Hi, Iām @infa-dabdulla
- š Iām interested in ...
- š± Iām currently learning ...
- šļø Iām looking to collaborate on ...
- š« How to reach me ...

<!---
infa-dabdulla/infa-dabdulla is a āØ special āØ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->




jenkins
apiVersion: v1
kind: Service
metadata:
  name: jenkinsserver
  labels:
    app: jenkins
    #tier: frontend
spec:
  type: LoadBalancer
  ports:
    # the port that this service should serve on
  - port: 80
    targetPort: 8080
  selector:
    app: jenkins
    #tier: frontend
