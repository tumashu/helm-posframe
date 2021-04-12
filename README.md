Note: this file is auto converted from helm-posframe.el by [el2org](https://github.com/tumashu/el2org), please do not edit it by hand!!!


# &#30446;&#24405;

1.  [helm-posframe README](#orgb70ade4)
    1.  [Need new maintainer !!!](#orgb2afcf6)
    2.  [What is helm-posframe](#org1386f89)
    3.  [How to enable helm-posframe](#orgf3839bc)
    4.  [Tips](#orgef17d6a)
        1.  [How to show fringe to helm-posframe](#org274c1ed)


<a id="orgb70ade4"></a>

# helm-posframe README


<a id="orgb2afcf6"></a>

## Need new maintainer !!!

I do not use helm and hard to maintain this package, for I
do not know the details of helm. need a new maintainer !!!


<a id="org1386f89"></a>

## What is helm-posframe

helm-posframe is a helm extension, which let helm use posframe
to show its candidate menu.

NOTE: helm-posframe requires Emacs 26


<a id="orgf3839bc"></a>

## How to enable helm-posframe

    (helm-posframe-enable)


<a id="orgef17d6a"></a>

## Tips


<a id="org274c1ed"></a>

### How to show fringe to helm-posframe

;; #+BEGIN\_EXAMPLE
(setq helm-posframe-parameters
      '((left-fringe . 10)
        (right-fringe . 10)))
;; #+END\_EXAMPLE

By the way, User can set **any** parameters of helm-posframe with
the help of \`helm-posframe-parameters'.

