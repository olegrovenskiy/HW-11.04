# HW-11.04

## Домашнее задание к занятию "11.04 Микросервисы: масштабирование"

Задача 1: Кластеризация
Предложите решение для обеспечения развертывания, запуска и управления приложениями. Решение может состоять из одного или нескольких программных продуктов и должно описывать способы и принципы их взаимодействия.

Моё предложение - внедрение кластера Kubernetes.

Из документации - 

Kubernetes is a portable, extensible, open-source platform for managing containerized workloads and services, that facilitates both declarative configuration and automation. It has a large, rapidly growing ecosystem. Kubernetes services, support, and tools are widely available.

Во первых это промышленное масштабируемое решение,

Во вторых оно удовлетворяет заявленным требованиям, ниже приведены тех. иребования и соответствующий функционал Kubernetes который обеспечивает их выполнение:


    Поддержка контейнеров;  Kubernetes как оркестратор для контейнеров
    Обеспечивать обнаружение сервисов и маршрутизацию запросов;  Cloud-native service discovery, Topology-aware traffic routing
    Обеспечивать возможность горизонтального масштабирования; Kubernetes Horizontal Pod Autoscaler
    Обеспечивать возможность автоматического масштабирования; Horizontal Pod Autoscaler обеспечивает масштабтрование на основе метрик
    Обеспечивать явное разделение ресурсов доступных извне и внутри системы; -- Resource Management for Pods and Containers
    Обеспечивать возможность конфигурировать приложения с помощью переменных среды, в том числе с возможностью безопасного хранения чувствительных данных таких как пароли, ключи доступа, ключи шифрования и т.п. -- обеспечивается различными вапиантами Secrets

В третьих это уже довольно зрелое решение, с 2014 года на рынке, которое - combines over 15 years of Google's experience running production workloads at scale with best-of-breed ideas and practices from the community.

