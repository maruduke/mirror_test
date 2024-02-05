---
title: '6. Reacive Programming'
excerpt: '리액티브 시스템'

categories:
    - MSA
tags:
    - [Spring, MSA]

permalink: /MSA/6

toc: true
toc_sticky: true

date: 2024-01-31
last_modified_at: 2024-01-31
---

## 1. 리액티브 시스템

기존 시스템의 경우, 요청이 들어왔을 경우 응답이 오기 전 까지 해당 쓰레드를 점유하는 동기 방식이었다. 해당 시스템은 JAVA가 트래픽 처리 성능에서 타 프레임워크에서 상당히 약세를 보였던 부분이다.  
해당 문제를 해결하기 위해서 요청을 비동기적으로 처리할 수 있는 방법이 리액티브 시스템으로 요청이 들어와도 쓰레드를 점유하지 않고 다른 요청을 처리하다 서버에서 응답이 왔을 경우 요청을 처리한다.

## 2. 리액티브 프로그래밍이란?

데이터 스트림과 변경사항 전파를 중심으로하는 비동기 프로그래밍 패러다임이다.

즉 데이터 스트림을 이용하여 전달하고, 데이터 변경시점을 이벤트로하여 수신자와 송신자 사이에 데이터를 전달시키는 비동기 프로그램이라고 한다.

## 3. 자료형 Mono, Flux

<!-- <img src="/assets/images/Kafka/1-4.png"> -->