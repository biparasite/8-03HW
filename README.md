# Домашнее задание к занятию "`GitLab`" - `Сулименков Алексей`

---

### Задание 1

####  gitlab-runner

Регистрация  gitlab-runner
![Регистрация gitlab-runner](https://github.com/biparasite/8-03HW/blob/main/8-03.1.1.png)

gitlab-runner
![gitlab-runner](https://github.com/biparasite/8-03HW/blob/main/8-03.1.2.png)

---

### Задание 2

#### 

Настройки gitlab-ci.yml 

```
stages:
  - test
  - build

test:
  stage: test
  image: golang:1.17
  script:
   - go test .

build:
  stage: build
  image: docker:latest
  script:
   - docker build .
```

Запуск сборки
![Запуск сборки](https://github.com/biparasite/8-03HW/blob/main/8-03.2.1.png)

---

