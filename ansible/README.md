CI/CD "Pipeline"
=========

Script for CI/CD, to build "student_age" image, then, deliver and deploy it.

CI
------------

`ansible-playbook -i inventory ci.yml`

ou

`ansible-playbook -i inventory ci.yml.vanilla`

CD
--------------

`ansible-playbook -i inventory cd.yml`

ou

`ansible-playbook -i inventory cd.yml.vanilla`

Dependencies
--------------

`ansible-playbook -i inventory cicd.yml`