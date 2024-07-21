가끔 개발을 하다보면 지금 브랜치를 최신 로컬 브랜치에 있는 변경사항을 모두 제거한 상태로 돌리고 싶은데 어떻게 하는지 까먹는 경우가 있다.
[GitKraken](https://www.gitkraken.com/lp/e3?utm_feeditemid=&utm_device=c&utm_term=gitkraken%20%EB%AC%B4%EB%A3%8C&utm_campaign=1+%7C+5+GK+Brand+-+Search&utm_source=google&utm_medium=ppc&hsa_acc=1130375851&hsa_cam=14828190375&hsa_grp=126688158646&hsa_ad=553348991700&hsa_src=g&hsa_tgt=kwd-2172108173673&hsa_kw=gitkraken%20%EB%AC%B4%EB%A3%8C&hsa_mt=b&hsa_net=adwords&hsa_ver=3&gad_source=1&gclid=CjwKCAjw4_K0BhBsEiwAfVVZ_xcyLkNMO1aBs-GoYk7DjrJFH_IeS1KgiHTcYccKCZxt7uytP7TD5xoC-HAQAvD_BwE)이나 [Source Tree](https://www.sourcetreeapp.com/)와 같은 툴을 사용하면 그나마 git 상태를 GUI로 볼 수 있어서 편한데 CLI는 어려울 수 있다.
그냥 `git reset --hard`를 사용하면 현재 브랜치에서 변경사항을 모두 폐기한다.
물론 해당 데이터는 즉시 소멸되기 때문에 복구하기 어려울 수 있다.
따라서 `git stash` 명령을 적극적으로 사용하면 좋다.