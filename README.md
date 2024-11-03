# rsschool-devops-course-tasks-app

## Task 4
https://github.com/rolling-scopes-school/tasks/blob/master/devops/modules/3_ci-configuration/task_4.md

Please use:
1. `kubectl apply -f jenkins-namespace.yaml`
2. `kubectl apply -f jenkins-volume.yaml`
3. `kubectl apply -f jenkins-serviceaccount.yaml`
commands to prepare kOps cluster for installation and then
4. `helm install jenkins -n jenkins -f jenkins-values.yaml jenkinsci/jenkins` and further `helm upgrade jenkins -n jenkins -f jenkins-values.yaml jenkinsci/jenkins`
commands from `k8s` directory to install Jenkins CI/CD instance fully configured and managed via YAML and JCasC.

JCasC configuration includes setup of regular Jenkins user and simple job (build) like freestyle project.
