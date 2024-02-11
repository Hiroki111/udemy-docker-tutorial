To use k8 on wsl2, I need to install kubectl on wsl2.
To do so, I need to use snapd (https://kubernetes.io/docs/tasks/tools/install-kubectl-linux/#install-using-other-package-management), but snapd isn't available on this machine. The status is always "unavailable".
https://forum.snapcraft.io/t/snap-d-error-cannot-communicate-with-server-connection-refused/6093

I'd probably need to reinstall ubuntu. Then, install snapd and kubectl.

I may not need to install minikube on wsl2: https://carmencincotti.com/2023-03-06/how-to-use-kubernetes-for-free-on-wsl/

