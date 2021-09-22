CI/CD "Pipeline"
=========

Script for CI/CD, to build "student_age" image, then, deliver and deploy it.

CI
------------
Put your docker pass in docker_pass.enc as:  
`docker_pass: <your_pass>`

Then, execute command:
`ansible-vault encrypt docker_pass.enc`

Edit the variables to you docker username,now you can run the script:

`ansible-playbook -i inventory -e @docker_pass.enc --ask-vault-pass ci.yml`

ou

`ansible-playbook -i inventory -e @docker_pass.enc --ask-vault-pass ci.yml.vanilla`

CD
--------------

`ansible-playbook -i inventory cd.yml`

ou

`ansible-playbook -i inventory cd.yml.vanilla`

CI & CD
--------------

`ansible-playbook -i inventory -i inventory -e @docker_pass.enc --ask-vault-pass cicd.yml`