Note: this file is auto converted from helm-posframe.el by [el2org](https://github.com/tumashu/el2org), please do not edit it by hand!!!


# &#30446;&#24405;

1.  [helm-posframe README](#orgc1a00ba)
    1.  [What is helm-posframe](#orga243ee0)
    2.  [How to enable helm-posframe](#org8c1ace2)
    3.  [Tips](#org60c7d25)
        1.  [How to show fringe to helm-posframe](#orge36a7d9)


<a id="orgc1a00ba"></a>

# helm-posframe README


<a id="orga243ee0"></a>

## What is helm-posframe

helm-posframe is a helm extension, which let helm use posframe
to show its candidate menu.

NOTE: helm-posframe requires Emacs 26


<a id="org8c1ace2"></a>

## How to enable helm-posframe

    (helm-posframe-enable)


<a id="org60c7d25"></a>

## Tips


<a id="orge36a7d9"></a>

### How to show fringe to helm-posframe

    (setq helm-posframe-parameters
          '((left-fringe . 10)
            (right-fringe . 10)))

By the way, User can set **any** parameters of helm-posframe with
the help of \`helm-posframe-parameters'.
