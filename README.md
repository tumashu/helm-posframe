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

## New maintainer!!!

 - Hey everyone! My name is OJ, and I am the new maintainer for helm-posframe!! I am here to help however you need, as best we can, as quick as I can! OJMac789@github.com or <ojandjess1@gmail.com>.
 - Please post your issues or pull requests and I will review asap. Also, feel free to email me!
   
   Cheers, OJ

<a id="org1386f89"></a>

## What is helm-posframe

helm-posframe is a helm extension, which let helm use posframe
to show its candidate menu.

NOTE: helm-posframe requires Emacs 26 or higher, helm, posframe


<a id="orgf3839bc"></a>

## How to enable helm-posframe

  1. Ensure you enable the helm-posframe package using your package manager e.g. use-package.
  2. Ensure you have the necessary dependencies installed for Emacs or Doom Emacs (helm, posframe, and Emacs 26+.)
  3. Clone this repo to your local machine in your home directory and follow the code example and path below to point Emacs to the helm-posframe repository.
  4. Add the code example below to your Doom Emacs config.el file:
  
    ;; Configure and enable "helm-posframe"
    (use-package! helm-posframe
    ;; :disabled t
    :after helm
    :demand t
    :if (and (window-system) (version<= "29.1" emacs-version))
    :config
    (setq helm-posframe-poshandler 'posframe-poshandler-frame-center
          helm-posframe-height 20
          helm-posframe-width (round (* (frame-width) 0.49))
          helm-posframe-parameters '((internal-border-width . 10)))
    (helm-posframe-enable)
  
      or add the code below to enable helm-posframe using your own configuration.

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

