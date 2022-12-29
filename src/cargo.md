# Cargo 사용하기

러스트에 대해 읽기 시작하면 머지않아 러스트 생태계에서 러스트 애플리케이션을 만들고 실행하는 데 사용되는 표준 도구인  [Cargo](https://doc.rust-lang.org/cargo/)를 만나게 될 것입니다. 여기서 우리는 Cargo가 무엇인지, 그리고 그것이 더 넓은 생태계에 어떻게 들어 맞는지, 그리고 그것이이 훈련에 어떻게 들어 맞는지에 대한 간략한 개요를 제공하고자 합니다.

데비안/우분투에서는 다음과 같이 Cargo와 Rust 소스를 설치할 수 있습니다.

```shell
$ sudo apt install cargo rust-src
```

이렇게 하면 [rust-analyzer][1] 가 정의로 이동할 수 있습니다. [VS Code][2] 를 사용하여 코드를 편집하는 것이 좋습니다(단, LSP 호환 편집기는 작동합니다).

참고로, 액세스/기능이 있다면 [rustup](https://rustup.rs/)을 통해 Rust의 툴링을 설치하는 것이 좋습니다. 이 툴링은 다른 에코시스템과 더 잘 통합되기 때문입니다.

[1]: https://rust-analyzer.github.io/
[2]: https://code.visualstudio.com/
