
Minimum viable product (MVP): R package `cats`
==============================================

서론
----

![cats](http://www.ipopcon.kr/public/upload/admin/thumbnail/20170213/4558a088ff26446e16cd0663608ded03.jpg)

R Programming 수강생 여러분들께

고양이를 좋아하는지 안좋아하는지 한줄로 출력하는 단순한 패키지입니다. ( [Minimum viable product](https://en.wikipedia.org/wiki/Minimum_viable_product) )

<https://hilaryparker.com/2014/04/29/writing-an-r-package-from-scratch/>

위 블로그 글에서 참고한 것으로, 상세한 설명은 위 링크를 참고하세요.

설치
----

설치는 다음과 같이 하면 됩니다.

``` r
install.packages("devtools")
devtools::install_github("shanmdphd/cats")
```

실행
----

실행은 다음과 같이 하면 됩니다.

``` r
library(cats)
cat_function()
```

    ## [1] "I love cats!"

``` r
cat_function(FALSE)
```

    ## [1] "I am not a cool person."

수정
----

CLI에서 `git clone https://github.com/shanmdphd/cats.git` 하거나 오른쪽 위의 초록색 버튼을 클릭해서 zip파일을 다운로드 한 뒤 압축을 풀고 소스를 수정 할 수 있습니다.

`roxygen2` 패키지를 사용하면 문서 작업을 쉽게 할 수 있습니다. 각 함수의 앞에 `#'` 으로 시작하는 주석을 각각 달고 다음의 함수를 실행하면 `NAMESPACE`와 `Rd` 파일을 자동으로 고쳐줍니다. 직접 Rd 파일을 수정하는 것보다 간소하다고 많은 사람들이 말하곤 합니다.

``` r
library(roxygen2)
roxygenize()
```
