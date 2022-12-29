# 코드를 Cargo와 함께 로컬로 실행

자신의 시스템에서 코드를 실험하려면 먼저 Rust를 설치해야 합니다. [instructions in the Rust Book][1]에 따라 이 작업을 수행합니다. 이것은 당신에게 동작하는 `rustc`와 `cargo`를 줄 것입니다. 글을 쓰는 시점에서 최신 안정 Rust 릴리스에는 이러한 버전이 있습니다.

```shell
% rustc --version
rustc 1.61.0 (fe5b13d68 2022-05-18)
% cargo --version
cargo 1.61.0 (a028ae4 2022-04-29)
```

이 절차를 수행한 후 다음 단계에 따라 이 교육의 예 중 하나에서 Rust 바이너리를 구축합니다.

1. 복사할 예제에서 "Copy to clipboard" 단추를 누릅니다.

2. `cargo new exercise`를 사용하여 코드에 대한 새 `exercise/` 디렉토리를 만듭니다.

    ```shell
    $ cargo new exercise
         Created binary (application) `exercise` package
    ```

3. `exercise/` 으로 이동하고 `cargo run` 을 사용하여 바이너리를 구축하고 실행합니다.

    ```shell
    $ cd exercise
    $ cargo run
       Compiling exercise v0.1.0 (/home/mgeisler/tmp/exercise)
        Finished dev [unoptimized + debuginfo] target(s) in 0.75s
         Running `target/debug/exercise`
    Hello, world!
    ```

4. `src/main.rs`의 보일러 플레이트 코드를 사용자 고유의 코드로 바꿉니다. 예를 들어, 이전 페이지의 예제를 사용하여 `src/main.rs`를 다음과 같이 만듭니다.

    ```rust
    fn main() {
        println!("Edit me!");
    }
    ```

5. `cargo run` 을 사용하여 업데이트된 이진 파일을 빌드하고 실행.

    ```shell
    $ cargo run
       Compiling exercise v0.1.0 (/home/mgeisler/tmp/exercise)
        Finished dev [unoptimized + debuginfo] target(s) in 0.24s
         Running `target/debug/exercise`
    Edit me!
    ```

6. Use `cargo check`를 사용하여 프로젝트의 오류를 신속하게 확인하고, `cargo build`를 사용하여 실행하지 않고 컴파일하십시오. 일반적인 디버그 빌드에 대한 출력은 `target/debug/` 에서 찾을 수 있습니다. `cargo build --release`를 사용하여 `target/release/`에서 최적화된 릴리스 빌드를 생성합니다.

7. `Cargo.toml`을 편집하여 프로젝트에 대한 종속성을 추가할 수 있습니다. `cargo` 명령을 실행하면 자동으로 누락 된 종속성을 다운로드하고 컴파일합니다.


[1]: https://doc.rust-lang.org/book/ch01-01-installation.html
