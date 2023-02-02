## 事前
```
source $HOME/.profile
```

## kernelビルド
```
cd $HOME/workspace/mikanos-of-the-ryo/kernel
source $HOME/osbook/devenv/buildenv.sh
make
```

## UEFIビルド
```
cd $HOME/edk2
source edksetup.sh
build
```

## QEMU実行
```
$HOME/osbook/devenv/run_qemu.sh Build/MikanLoaderX64/DEBUG_CLANG38/X64/Loader.efi $HOME/workspace/mikanos-of-the-ryo/kernel/kernel.elf
```

## tag比較
```
git diff --name-only --diff-filter=AMCRD tag1 tag2
```

## appまとめて実行
```
cd $HOME/workspace/mikanos-of-the-ryo
source $HOME/.profile
source $HOME/osbook/devenv/buildenv.sh
source buid.sh run
```