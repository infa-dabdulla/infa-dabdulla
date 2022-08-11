- 👋 Hi, I’m @infa-dabdulla
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
infa-dabdulla/infa-dabdulla is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
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
