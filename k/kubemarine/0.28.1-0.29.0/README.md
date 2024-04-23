# Comparing `tmp/kubemarine-0.28.1.tar.gz` & `tmp/kubemarine-0.29.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kubemarine-0.28.1.tar", last modified: Mon Apr  1 09:25:06 2024, max compression
+gzip compressed data, was "kubemarine-0.29.0.tar", last modified: Fri Apr 19 15:14:25 2024, max compression
```

## Comparing `kubemarine-0.28.1.tar` & `kubemarine-0.29.0.tar`

### file list

```diff
@@ -1,272 +1,276 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.132035 kubemarine-0.28.1/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-04-01 09:24:41.000000 kubemarine-0.28.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      183 2024-04-01 09:24:41.000000 kubemarine-0.28.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    13978 2024-04-01 09:25:06.132035 kubemarine-0.28.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9311 2024-04-01 09:24:41.000000 kubemarine-0.28.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.064035 kubemarine-0.28.1/bin/
--rwxr-xr-x   0 root         (0) root         (0)     1076 2024-04-01 09:24:41.000000 kubemarine-0.28.1/bin/kubemarine
--rw-r--r--   0 root         (0) root         (0)      657 2024-04-01 09:24:41.000000 kubemarine-0.28.1/bin/kubemarine.cmd
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.072035 kubemarine-0.28.1/kubemarine/
--rw-r--r--   0 root         (0) root         (0)      603 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     7924 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/__main__.py
--rw-r--r--   0 root         (0) root         (0)    29086 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/admission.py
--rw-r--r--   0 root         (0) root         (0)     5625 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/apparmor.py
--rw-r--r--   0 root         (0) root         (0)     5517 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/apt.py
--rw-r--r--   0 root         (0) root         (0)     6228 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/audit.py
--rw-r--r--   0 root         (0) root         (0)     2203 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/controlplane.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.076035 kubemarine-0.28.1/kubemarine/core/
--rw-r--r--   0 root         (0) root         (0)      604 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2044 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/core/action.py
--rw-r--r--   0 root         (0) root         (0)     2151 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/core/annotations.py
--rwxr-xr-x   0 root         (0) root         (0)    28019 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/core/cluster.py
--rw-r--r--   0 root         (0) root         (0)     4224 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/core/connections.py
--rwxr-xr-x   0 root         (0) root         (0)    28358 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/core/defaults.py
--rw-r--r--   0 root         (0) root         (0)     1125 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/core/environment.py
--rw-r--r--   0 root         (0) root         (0)     7299 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/core/errors.py
--rw-r--r--   0 root         (0) root         (0)    30247 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/core/executor.py
--rwxr-xr-x   0 root         (0) root         (0)    21799 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/core/flow.py
--rwxr-xr-x   0 root         (0) root         (0)    38504 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/core/group.py
--rw-r--r--   0 root         (0) root         (0)    15334 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/core/log.py
--rw-r--r--   0 root         (0) root         (0)     1060 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/core/os.py
--rw-r--r--   0 root         (0) root         (0)     2640 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/core/patch.py
--rw-r--r--   0 root         (0) root         (0)    24538 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/core/resources.py
--rw-r--r--   0 root         (0) root         (0)    15524 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/core/schema.py
--rw-r--r--   0 root         (0) root         (0)     2412 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/core/static.py
--rw-r--r--   0 root         (0) root         (0)     2183 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/core/summary.py
--rwxr-xr-x   0 root         (0) root         (0)    26348 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/core/utils.py
--rw-r--r--   0 root         (0) root         (0)     1993 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/core/yaml_merger.py
--rw-r--r--   0 root         (0) root         (0)     7230 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/coredns.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.080035 kubemarine-0.28.1/kubemarine/cri/
--rw-r--r--   0 root         (0) root         (0)     3373 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/cri/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    16741 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/cri/containerd.py
--rwxr-xr-x   0 root         (0) root         (0)     3892 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/cri/docker.py
--rw-r--r--   0 root         (0) root         (0)    27236 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/demo.py
--rw-r--r--   0 root         (0) root         (0)     4648 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/etcd.py
--rw-r--r--   0 root         (0) root         (0)    10637 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/haproxy.py
--rw-r--r--   0 root         (0) root         (0)     2734 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/jinja.py
--rw-r--r--   0 root         (0) root         (0)     2347 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/k8s_certs.py
--rw-r--r--   0 root         (0) root         (0)    12492 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/keepalived.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.080035 kubemarine-0.28.1/kubemarine/kubernetes/
--rw-r--r--   0 root         (0) root         (0)    55178 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/kubernetes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    47459 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/kubernetes/components.py
--rw-r--r--   0 root         (0) root         (0)     2219 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/kubernetes/daemonset.py
--rw-r--r--   0 root         (0) root         (0)     1783 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/kubernetes/deployment.py
--rw-r--r--   0 root         (0) root         (0)     3993 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/kubernetes/object.py
--rw-r--r--   0 root         (0) root         (0)     2162 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/kubernetes/replicaset.py
--rw-r--r--   0 root         (0) root         (0)     4342 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/kubernetes/secrets.py
--rw-r--r--   0 root         (0) root         (0)     2007 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/kubernetes/statefulset.py
--rw-r--r--   0 root         (0) root         (0)     5945 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/kubernetes_accounts.py
--rw-r--r--   0 root         (0) root         (0)     4007 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/modprobe.py
--rw-r--r--   0 root         (0) root         (0)    30768 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/packages.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.080035 kubemarine-0.28.1/kubemarine/patches/
--rw-r--r--   0 root         (0) root         (0)     1224 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/patches/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2246 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/patches/patch_kubelet_configmap.py
--rw-r--r--   0 root         (0) root         (0)     1036 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/patches/software_upgrade.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.084035 kubemarine-0.28.1/kubemarine/plugins/
--rwxr-xr-x   0 root         (0) root         (0)    44549 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7859 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/builtin.py
--rwxr-xr-x   0 root         (0) root         (0)    29024 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/calico.py
--rw-r--r--   0 root         (0) root         (0)     7889 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/kubernetes_dashboard.py
--rw-r--r--   0 root         (0) root         (0)     7928 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/local_path_provisioner.py
--rw-r--r--   0 root         (0) root         (0)    27745 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/manifest.py
--rw-r--r--   0 root         (0) root         (0)    19679 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/nginx_ingress.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.092035 kubemarine-0.28.1/kubemarine/plugins/yaml/
--rw-r--r--   0 root         (0) root         (0)     5796 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/calico-apiserver-v3.24.2-original.yaml
--rw-r--r--   0 root         (0) root         (0)     5874 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/calico-apiserver-v3.25.1-original.yaml
--rw-r--r--   0 root         (0) root         (0)     5886 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/calico-apiserver-v3.26.1-original.yaml
--rw-r--r--   0 root         (0) root         (0)     5886 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/calico-apiserver-v3.26.4-original.yaml
--rw-r--r--   0 root         (0) root         (0)     5886 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/calico-apiserver-v3.27.0-original.yaml
--rw-r--r--   0 root         (0) root         (0)   222019 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/calico-v3.22.2-original.yaml
--rw-r--r--   0 root         (0) root         (0)   239857 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/calico-v3.24.2-original.yaml
--rw-r--r--   0 root         (0) root         (0)   243952 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/calico-v3.25.1-original.yaml
--rw-r--r--   0 root         (0) root         (0)   250597 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/calico-v3.26.1-original.yaml
--rw-r--r--   0 root         (0) root         (0)   250781 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/calico-v3.26.4-original.yaml
--rw-r--r--   0 root         (0) root         (0)   258410 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/calico-v3.27.0-original.yaml
--rw-r--r--   0 root         (0) root         (0)     7621 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/kubernetes-dashboard-v2.5.1-original.yaml
--rw-r--r--   0 root         (0) root         (0)     7621 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/kubernetes-dashboard-v2.7.0-original.yaml
--rw-r--r--   0 root         (0) root         (0)     2935 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/local-path-provisioner-v0.0.22-original.yaml
--rw-r--r--   0 root         (0) root         (0)     2935 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/local-path-provisioner-v0.0.23-original.yaml
--rw-r--r--   0 root         (0) root         (0)     2935 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/local-path-provisioner-v0.0.24-original.yaml
--rw-r--r--   0 root         (0) root         (0)     3752 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/local-path-provisioner-v0.0.25-original.yaml
--rw-r--r--   0 root         (0) root         (0)     3752 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/local-path-provisioner-v0.0.26-original.yaml
--rw-r--r--   0 root         (0) root         (0)    15311 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/nginx-ingress-controller-v1.2.0-original.yaml
--rw-r--r--   0 root         (0) root         (0)    15775 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/nginx-ingress-controller-v1.4.0-original.yaml
--rw-r--r--   0 root         (0) root         (0)    15704 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/nginx-ingress-controller-v1.7.0-original.yaml
--rw-r--r--   0 root         (0) root         (0)    15642 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/nginx-ingress-controller-v1.8.1-original.yaml
--rw-r--r--   0 root         (0) root         (0)    15662 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/nginx-ingress-controller-v1.8.4-original.yaml
--rw-r--r--   0 root         (0) root         (0)    16337 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/nginx-ingress-controller-v1.9.4-original.yaml
--rw-r--r--   0 root         (0) root         (0)    16107 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/nginx-ingress-controller-v1.9.5-original.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.096035 kubemarine-0.28.1/kubemarine/procedures/
--rw-r--r--   0 root         (0) root         (0)     3369 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/procedures/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     4643 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/procedures/add_node.py
--rwxr-xr-x   0 root         (0) root         (0)    32509 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/procedures/backup.py
--rwxr-xr-x   0 root         (0) root         (0)     3553 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/procedures/cert_renew.py
--rwxr-xr-x   0 root         (0) root         (0)    73784 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/procedures/check_iaas.py
--rwxr-xr-x   0 root         (0) root         (0)    90567 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/procedures/check_paas.py
--rw-r--r--   0 root         (0) root         (0)     2719 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/procedures/config.py
--rwxr-xr-x   0 root         (0) root         (0)     4891 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/procedures/do.py
--rwxr-xr-x   0 root         (0) root         (0)    23256 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/procedures/install.py
--rwxr-xr-x   0 root         (0) root         (0)     1643 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/procedures/manage_psp.py
--rwxr-xr-x   0 root         (0) root         (0)     1532 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/procedures/manage_pss.py
--rwxr-xr-x   0 root         (0) root         (0)     8120 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/procedures/migrate_cri.py
--rw-r--r--   0 root         (0) root         (0)    21620 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/procedures/migrate_kubemarine.py
--rwxr-xr-x   0 root         (0) root         (0)     2435 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/procedures/reboot.py
--rw-r--r--   0 root         (0) root         (0)     2607 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/procedures/reconfigure.py
--rwxr-xr-x   0 root         (0) root         (0)     3928 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/procedures/remove_node.py
--rwxr-xr-x   0 root         (0) root         (0)    14156 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/procedures/restore.py
--rwxr-xr-x   0 root         (0) root         (0)    13035 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/procedures/upgrade.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.096035 kubemarine-0.28.1/kubemarine/resources/
--rw-r--r--   0 root         (0) root         (0)      604 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.100035 kubemarine-0.28.1/kubemarine/resources/configurations/
--rw-r--r--   0 root         (0) root         (0)      604 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/configurations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.100035 kubemarine-0.28.1/kubemarine/resources/configurations/compatibility/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.100035 kubemarine-0.28.1/kubemarine/resources/configurations/compatibility/internal/
--rw-r--r--   0 root         (0) root         (0)     4716 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/configurations/compatibility/internal/kubernetes_images.yaml
--rw-r--r--   0 root         (0) root         (0)     5889 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/configurations/compatibility/internal/packages.yaml
--rw-r--r--   0 root         (0) root         (0)     5025 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/configurations/compatibility/internal/plugins.yaml
--rw-r--r--   0 root         (0) root         (0)     7663 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/configurations/compatibility/internal/thirdparties.yaml
--rw-r--r--   0 root         (0) root         (0)     3944 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/configurations/compatibility/kubernetes_versions.yaml
--rw-r--r--   0 root         (0) root         (0)    31923 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/configurations/defaults.yaml
--rw-r--r--   0 root         (0) root         (0)    11291 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/configurations/globals.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.100035 kubemarine-0.28.1/kubemarine/resources/drop_ins/
--rw-r--r--   0 root         (0) root         (0)      604 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/drop_ins/__init__.py
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/drop_ins/haproxy.conf
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/drop_ins/keepalived.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.060035 kubemarine-0.28.1/kubemarine/resources/etalons/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.100035 kubemarine-0.28.1/kubemarine/resources/etalons/patches/
--rw-r--r--   0 root         (0) root         (0)     1126 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/etalons/patches/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1036 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/etalons/patches/software_upgrade.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.104035 kubemarine-0.28.1/kubemarine/resources/psp/
--rw-r--r--   0 root         (0) root         (0)      604 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/psp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1457 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/psp/anyuid.yaml
--rw-r--r--   0 root         (0) root         (0)     1923 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/psp/default.yaml
--rw-r--r--   0 root         (0) root         (0)     1618 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/psp/host-network.yaml
--rw-r--r--   0 root         (0) root         (0)     1204 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/psp/privileged.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.104035 kubemarine-0.28.1/kubemarine/resources/reports/
--rw-r--r--   0 root         (0) root         (0)      604 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/reports/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1773 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/reports/check_report.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.108035 kubemarine-0.28.1/kubemarine/resources/schemas/
--rw-r--r--   0 root         (0) root         (0)      478 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/add_node.json
--rw-r--r--   0 root         (0) root         (0)     2643 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/backup.json
--rw-r--r--   0 root         (0) root         (0)     1635 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/cert_renew.json
--rw-r--r--   0 root         (0) root         (0)      415 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/check_paas.json
--rw-r--r--   0 root         (0) root         (0)     3142 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/cluster.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.108035 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.112035 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/common/
--rw-r--r--   0 root         (0) root         (0)     1429 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/common/node_ref.json
--rw-r--r--   0 root         (0) root         (0)     1722 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/common/utils.json
--rw-r--r--   0 root         (0) root         (0)      708 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/gateway_node.json
--rw-r--r--   0 root         (0) root         (0)     4072 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/globals.json
--rw-r--r--   0 root         (0) root         (0)     1501 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/node.json
--rw-r--r--   0 root         (0) root         (0)     2363 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/node_defaults.json
--rw-r--r--   0 root         (0) root         (0)      575 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugin_defaults.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.112035 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/
--rw-r--r--   0 root         (0) root         (0)     7227 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/calico.json
--rw-r--r--   0 root         (0) root         (0)     2009 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/generic_plugin.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.112035 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/installation/
--rw-r--r--   0 root         (0) root         (0)     1278 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/installation/ansible.json
--rw-r--r--   0 root         (0) root         (0)      689 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/installation/config.json
--rw-r--r--   0 root         (0) root         (0)     3120 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/installation/expect.json
--rw-r--r--   0 root         (0) root         (0)     1220 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/installation/helm.json
--rw-r--r--   0 root         (0) root         (0)      606 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/installation/python.json
--rw-r--r--   0 root         (0) root         (0)     2265 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/installation/shell.json
--rw-r--r--   0 root         (0) root         (0)     2498 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/installation/template.json
--rw-r--r--   0 root         (0) root         (0)     1780 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/installation.json
--rw-r--r--   0 root         (0) root         (0)     3129 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/kubernetes-dashboard.json
--rw-r--r--   0 root         (0) root         (0)     1743 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/local-path-provisioner.json
--rw-r--r--   0 root         (0) root         (0)     3472 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/nginx-ingress-controller.json
--rw-r--r--   0 root         (0) root         (0)      605 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins.json
--rw-r--r--   0 root         (0) root         (0)      749 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/procedures.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.116035 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/rbac/
--rw-r--r--   0 root         (0) root         (0)      661 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/rbac/account.json
--rw-r--r--   0 root         (0) root         (0)     3266 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/rbac/account_defaults.json
--rw-r--r--   0 root         (0) root         (0)     3759 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/rbac/psp.json
--rw-r--r--   0 root         (0) root         (0)     2453 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/rbac/pss.json
--rw-r--r--   0 root         (0) root         (0)      709 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/rbac.json
--rw-r--r--   0 root         (0) root         (0)     1951 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/registry.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.120035 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/
--rw-r--r--   0 root         (0) root         (0)     1948 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/audit.json
--rw-r--r--   0 root         (0) root         (0)     9668 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/coredns.json
--rw-r--r--   0 root         (0) root         (0)     3115 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/cri.json
--rw-r--r--   0 root         (0) root         (0)      644 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/etc_hosts.json
--rw-r--r--   0 root         (0) root         (0)     1963 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/kernel_security.json
--rw-r--r--   0 root         (0) root         (0)     5430 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/kubeadm.json
--rw-r--r--   0 root         (0) root         (0)      998 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/kubeadm_kube-proxy.json
--rw-r--r--   0 root         (0) root         (0)      938 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/kubeadm_kubelet.json
--rw-r--r--   0 root         (0) root         (0)     2764 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/kubeadm_patches.json
--rw-r--r--   0 root         (0) root         (0)     5264 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/loadbalancer.json
--rw-r--r--   0 root         (0) root         (0)     1001 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/modprobe.json
--rw-r--r--   0 root         (0) root         (0)     2302 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/ntp.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.120035 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/packages/
--rw-r--r--   0 root         (0) root         (0)     4268 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/packages/associations.json
--rw-r--r--   0 root         (0) root         (0)     5144 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/packages.json
--rw-r--r--   0 root         (0) root         (0)      479 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/resolv.conf.json
--rw-r--r--   0 root         (0) root         (0)     1243 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/sysctl.json
--rw-r--r--   0 root         (0) root         (0)     3302 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/thirdparties.json
--rw-r--r--   0 root         (0) root         (0)     1965 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services.json
--rw-r--r--   0 root         (0) root         (0)     3130 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/vrrp_ip.json
--rw-r--r--   0 root         (0) root         (0)      757 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/manage_psp.json
--rw-r--r--   0 root         (0) root         (0)     1657 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/manage_pss.json
--rw-r--r--   0 root         (0) root         (0)     1749 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/migrate_cri.json
--rw-r--r--   0 root         (0) root         (0)     2885 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/migrate_kubemarine.json
--rw-r--r--   0 root         (0) root         (0)      798 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/reboot.json
--rw-r--r--   0 root         (0) root         (0)     2326 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/reconfigure.json
--rw-r--r--   0 root         (0) root         (0)      872 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/remove_node.json
--rw-r--r--   0 root         (0) root         (0)     3365 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/restore.json
--rw-r--r--   0 root         (0) root         (0)     3504 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/upgrade.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.124035 kubemarine-0.28.1/kubemarine/resources/scripts/
--rw-r--r--   0 root         (0) root         (0)      604 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/scripts/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      288 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/scripts/check_haproxy.sh
--rw-r--r--   0 root         (0) root         (0)     1814 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/scripts/check_url_availability.py
--rwxr-xr-x   0 root         (0) root         (0)     3646 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/scripts/etcdctl.sh
--rwxr-xr-x   0 root         (0) root         (0)  2664796 2024-04-01 09:25:00.000000 kubemarine-0.28.1/kubemarine/resources/scripts/ipip_check.gz
--rw-r--r--   0 root         (0) root         (0)     1483 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/scripts/simple_port_client.py
--rw-r--r--   0 root         (0) root         (0)     2022 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/scripts/simple_port_listener.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.060035 kubemarine-0.28.1/kubemarine/resources/scripts/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.124035 kubemarine-0.28.1/kubemarine/resources/scripts/source/ipip_check/
--rw-r--r--   0 root         (0) root         (0)       71 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/scripts/source/ipip_check/go.mod
--rw-r--r--   0 root         (0) root         (0)     1446 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/scripts/source/ipip_check/go.sum
--rw-r--r--   0 root         (0) root         (0)     5732 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/scripts/source/ipip_check/ipip_check.go
--rw-r--r--   0 root         (0) root         (0)     8542 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/selinux.py
--rw-r--r--   0 root         (0) root         (0)     4073 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/sysctl.py
--rw-r--r--   0 root         (0) root         (0)    26273 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/system.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.128035 kubemarine-0.28.1/kubemarine/templates/
--rw-r--r--   0 root         (0) root         (0)      604 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)      667 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/templates/admission.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     2431 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/templates/haproxy.cfg.j2
--rw-r--r--   0 root         (0) root         (0)      996 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/templates/keepalived.conf.j2
--rw-r--r--   0 root         (0) root         (0)     1126 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/templates/kubelet.service.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.128035 kubemarine-0.28.1/kubemarine/templates/patches/
--rw-r--r--   0 root         (0) root         (0)      151 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/templates/patches/control-plane-pod.json.j2
--rw-r--r--   0 root         (0) root         (0)       76 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/templates/patches/kubelet.yaml.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.132035 kubemarine-0.28.1/kubemarine/templates/plugins/
--rw-r--r--   0 root         (0) root         (0)      604 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/templates/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)      879 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/templates/plugins/calico-ippool.yaml.j2
--rw-r--r--   0 root         (0) root         (0)      286 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/templates/plugins/calico-kube-controllers-metrics.yaml
--rw-r--r--   0 root         (0) root         (0)      245 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/templates/plugins/calico-metrics.yaml
--rw-r--r--   0 root         (0) root         (0)      436 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/templates/plugins/calico-rr.sh.j2
--rw-r--r--   0 root         (0) root         (0)      960 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/templates/plugins/calico-rr.yaml.j2
--rw-r--r--   0 root         (0) root         (0)      262 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/templates/plugins/calico-typha-metrics.yaml
--rw-r--r--   0 root         (0) root         (0)      136 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/templates/plugins/calicoctl.cfg.j2
--rw-r--r--   0 root         (0) root         (0)      107 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/templates/plugins/dashboard-ingress.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     8826 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/templates/plugins/dashboard-v2.5.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     8905 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/templates/plugins/dashboard-v2.7.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     2749 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/templates/plugins/iperf3.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     5401 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/templates/plugins/local-path-provisioner.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     9973 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/templates/plugins/nginx-ingress-controller-v1.2.yaml.j2
--rw-r--r--   0 root         (0) root         (0)    17847 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/templates/plugins/nginx-ingress-controller-v1.4.yaml.j2
--rw-r--r--   0 root         (0) root         (0)    11852 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/testsuite.py
--rw-r--r--   0 root         (0) root         (0)    19546 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/thirdparties.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/version
--rw-r--r--   0 root         (0) root         (0)     5696 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/yum.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.132035 kubemarine-0.28.1/kubemarine.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13978 2024-04-01 09:25:06.000000 kubemarine-0.28.1/kubemarine.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10671 2024-04-01 09:25:06.000000 kubemarine-0.28.1/kubemarine.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-01 09:25:06.000000 kubemarine-0.28.1/kubemarine.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2024-04-01 09:25:06.000000 kubemarine-0.28.1/kubemarine.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      492 2024-04-01 09:25:06.000000 kubemarine-0.28.1/kubemarine.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-04-01 09:25:06.000000 kubemarine-0.28.1/kubemarine.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     3535 2024-04-01 09:24:41.000000 kubemarine-0.28.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-01 09:25:06.132035 kubemarine-0.28.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1628 2024-04-01 09:24:41.000000 kubemarine-0.28.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.860358 kubemarine-0.29.0/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-04-19 15:14:01.000000 kubemarine-0.29.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      183 2024-04-19 15:14:01.000000 kubemarine-0.29.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    14049 2024-04-19 15:14:25.860358 kubemarine-0.29.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9311 2024-04-19 15:14:01.000000 kubemarine-0.29.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.792358 kubemarine-0.29.0/bin/
+-rwxr-xr-x   0 root         (0) root         (0)     1076 2024-04-19 15:14:01.000000 kubemarine-0.29.0/bin/kubemarine
+-rw-r--r--   0 root         (0) root         (0)      657 2024-04-19 15:14:01.000000 kubemarine-0.29.0/bin/kubemarine.cmd
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.800358 kubemarine-0.29.0/kubemarine/
+-rw-r--r--   0 root         (0) root         (0)      603 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     7973 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    28959 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/admission.py
+-rw-r--r--   0 root         (0) root         (0)     5506 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/apparmor.py
+-rw-r--r--   0 root         (0) root         (0)     5517 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/apt.py
+-rw-r--r--   0 root         (0) root         (0)     6228 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/audit.py
+-rw-r--r--   0 root         (0) root         (0)     2203 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/controlplane.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.804358 kubemarine-0.29.0/kubemarine/core/
+-rw-r--r--   0 root         (0) root         (0)      604 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2043 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/core/action.py
+-rw-r--r--   0 root         (0) root         (0)     2151 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/core/annotations.py
+-rwxr-xr-x   0 root         (0) root         (0)    29983 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/core/cluster.py
+-rw-r--r--   0 root         (0) root         (0)     4292 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/core/connections.py
+-rwxr-xr-x   0 root         (0) root         (0)    30924 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/core/defaults.py
+-rw-r--r--   0 root         (0) root         (0)     1044 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/core/environment.py
+-rw-r--r--   0 root         (0) root         (0)     7314 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/core/errors.py
+-rw-r--r--   0 root         (0) root         (0)    30562 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/core/executor.py
+-rwxr-xr-x   0 root         (0) root         (0)    21097 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/core/flow.py
+-rwxr-xr-x   0 root         (0) root         (0)    38592 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/core/group.py
+-rw-r--r--   0 root         (0) root         (0)    15382 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/core/log.py
+-rw-r--r--   0 root         (0) root         (0)     1060 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/core/os.py
+-rw-r--r--   0 root         (0) root         (0)     2729 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/core/patch.py
+-rw-r--r--   0 root         (0) root         (0)    24931 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/core/resources.py
+-rw-r--r--   0 root         (0) root         (0)    16671 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/core/schema.py
+-rw-r--r--   0 root         (0) root         (0)     2345 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/core/static.py
+-rw-r--r--   0 root         (0) root         (0)     2185 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/core/summary.py
+-rwxr-xr-x   0 root         (0) root         (0)    26382 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/core/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1988 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/core/yaml_merger.py
+-rw-r--r--   0 root         (0) root         (0)     7218 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/coredns.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.808358 kubemarine-0.29.0/kubemarine/cri/
+-rw-r--r--   0 root         (0) root         (0)     3373 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/cri/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    16782 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/cri/containerd.py
+-rwxr-xr-x   0 root         (0) root         (0)     3892 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/cri/docker.py
+-rw-r--r--   0 root         (0) root         (0)    27748 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/demo.py
+-rw-r--r--   0 root         (0) root         (0)     4619 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/etcd.py
+-rw-r--r--   0 root         (0) root         (0)    10637 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/haproxy.py
+-rw-r--r--   0 root         (0) root         (0)     2993 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/jinja.py
+-rw-r--r--   0 root         (0) root         (0)     2347 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/k8s_certs.py
+-rw-r--r--   0 root         (0) root         (0)    12441 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/keepalived.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.808358 kubemarine-0.29.0/kubemarine/kubernetes/
+-rw-r--r--   0 root         (0) root         (0)    55462 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/kubernetes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    47459 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/kubernetes/components.py
+-rw-r--r--   0 root         (0) root         (0)     2219 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/kubernetes/daemonset.py
+-rw-r--r--   0 root         (0) root         (0)     1783 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/kubernetes/deployment.py
+-rw-r--r--   0 root         (0) root         (0)     3993 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/kubernetes/object.py
+-rw-r--r--   0 root         (0) root         (0)     2162 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/kubernetes/replicaset.py
+-rw-r--r--   0 root         (0) root         (0)     4342 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/kubernetes/secrets.py
+-rw-r--r--   0 root         (0) root         (0)     2007 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/kubernetes/statefulset.py
+-rw-r--r--   0 root         (0) root         (0)     5967 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/kubernetes_accounts.py
+-rw-r--r--   0 root         (0) root         (0)     4007 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/modprobe.py
+-rw-r--r--   0 root         (0) root         (0)    30835 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/packages.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.808358 kubemarine-0.29.0/kubemarine/patches/
+-rw-r--r--   0 root         (0) root         (0)     1371 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/patches/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/patches/boot_timeout_per_node.py
+-rw-r--r--   0 root         (0) root         (0)     1045 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/patches/software_upgrade.yaml
+-rw-r--r--   0 root         (0) root         (0)     1569 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/patches/strong_cipher_suits_for_kubelet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.812358 kubemarine-0.29.0/kubemarine/plugins/
+-rwxr-xr-x   0 root         (0) root         (0)    44984 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7859 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/builtin.py
+-rwxr-xr-x   0 root         (0) root         (0)    29039 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/calico.py
+-rw-r--r--   0 root         (0) root         (0)     7916 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/kubernetes_dashboard.py
+-rw-r--r--   0 root         (0) root         (0)     7942 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/local_path_provisioner.py
+-rw-r--r--   0 root         (0) root         (0)    27778 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/manifest.py
+-rw-r--r--   0 root         (0) root         (0)    19641 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/nginx_ingress.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.820358 kubemarine-0.29.0/kubemarine/plugins/yaml/
+-rw-r--r--   0 root         (0) root         (0)     5796 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/calico-apiserver-v3.24.2-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     5874 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/calico-apiserver-v3.25.1-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     5886 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/calico-apiserver-v3.26.1-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     5886 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/calico-apiserver-v3.26.4-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     5886 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/calico-apiserver-v3.27.0-original.yaml
+-rw-r--r--   0 root         (0) root         (0)   222019 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/calico-v3.22.2-original.yaml
+-rw-r--r--   0 root         (0) root         (0)   239857 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/calico-v3.24.2-original.yaml
+-rw-r--r--   0 root         (0) root         (0)   243952 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/calico-v3.25.1-original.yaml
+-rw-r--r--   0 root         (0) root         (0)   250597 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/calico-v3.26.1-original.yaml
+-rw-r--r--   0 root         (0) root         (0)   250781 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/calico-v3.26.4-original.yaml
+-rw-r--r--   0 root         (0) root         (0)   258410 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/calico-v3.27.0-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     7621 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.5.1-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     7621 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.7.0-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     2935 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.22-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     2935 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.23-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     2935 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.24-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     3752 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.25-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     3752 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.26-original.yaml
+-rw-r--r--   0 root         (0) root         (0)    15311 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.2.0-original.yaml
+-rw-r--r--   0 root         (0) root         (0)    15775 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.4.0-original.yaml
+-rw-r--r--   0 root         (0) root         (0)    15704 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.7.0-original.yaml
+-rw-r--r--   0 root         (0) root         (0)    15642 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.8.1-original.yaml
+-rw-r--r--   0 root         (0) root         (0)    15662 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.8.4-original.yaml
+-rw-r--r--   0 root         (0) root         (0)    16337 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.9.4-original.yaml
+-rw-r--r--   0 root         (0) root         (0)    16107 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.9.5-original.yaml
+-rw-r--r--   0 root         (0) root         (0)    16107 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.9.6-original.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.824358 kubemarine-0.29.0/kubemarine/procedures/
+-rw-r--r--   0 root         (0) root         (0)     3369 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/procedures/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     4643 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/procedures/add_node.py
+-rwxr-xr-x   0 root         (0) root         (0)    32557 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/procedures/backup.py
+-rwxr-xr-x   0 root         (0) root         (0)     3553 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/procedures/cert_renew.py
+-rwxr-xr-x   0 root         (0) root         (0)    73258 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/procedures/check_iaas.py
+-rwxr-xr-x   0 root         (0) root         (0)    90763 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/procedures/check_paas.py
+-rw-r--r--   0 root         (0) root         (0)     2747 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/procedures/config.py
+-rwxr-xr-x   0 root         (0) root         (0)     5004 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/procedures/do.py
+-rwxr-xr-x   0 root         (0) root         (0)    23627 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/procedures/install.py
+-rwxr-xr-x   0 root         (0) root         (0)     1643 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/procedures/manage_psp.py
+-rwxr-xr-x   0 root         (0) root         (0)     1532 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/procedures/manage_pss.py
+-rwxr-xr-x   0 root         (0) root         (0)     8057 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/procedures/migrate_cri.py
+-rw-r--r--   0 root         (0) root         (0)    21667 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/procedures/migrate_kubemarine.py
+-rwxr-xr-x   0 root         (0) root         (0)     2435 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/procedures/reboot.py
+-rw-r--r--   0 root         (0) root         (0)     2607 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/procedures/reconfigure.py
+-rwxr-xr-x   0 root         (0) root         (0)     3928 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/procedures/remove_node.py
+-rwxr-xr-x   0 root         (0) root         (0)    14178 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/procedures/restore.py
+-rwxr-xr-x   0 root         (0) root         (0)    13025 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/procedures/upgrade.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.824358 kubemarine-0.29.0/kubemarine/resources/
+-rw-r--r--   0 root         (0) root         (0)      604 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.828358 kubemarine-0.29.0/kubemarine/resources/configurations/
+-rw-r--r--   0 root         (0) root         (0)      604 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/configurations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.828358 kubemarine-0.29.0/kubemarine/resources/configurations/compatibility/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.828358 kubemarine-0.29.0/kubemarine/resources/configurations/compatibility/internal/
+-rw-r--r--   0 root         (0) root         (0)     4939 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/configurations/compatibility/internal/kubernetes_images.yaml
+-rw-r--r--   0 root         (0) root         (0)     6152 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/configurations/compatibility/internal/packages.yaml
+-rw-r--r--   0 root         (0) root         (0)     5256 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/configurations/compatibility/internal/plugins.yaml
+-rw-r--r--   0 root         (0) root         (0)     8015 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/configurations/compatibility/internal/thirdparties.yaml
+-rw-r--r--   0 root         (0) root         (0)     4101 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/configurations/compatibility/kubernetes_versions.yaml
+-rw-r--r--   0 root         (0) root         (0)    32236 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/configurations/defaults.yaml
+-rw-r--r--   0 root         (0) root         (0)    11309 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/configurations/globals.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.828358 kubemarine-0.29.0/kubemarine/resources/drop_ins/
+-rw-r--r--   0 root         (0) root         (0)      604 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/drop_ins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/drop_ins/haproxy.conf
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/drop_ins/keepalived.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.788358 kubemarine-0.29.0/kubemarine/resources/etalons/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.828358 kubemarine-0.29.0/kubemarine/resources/etalons/patches/
+-rw-r--r--   0 root         (0) root         (0)     1126 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/etalons/patches/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1036 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/etalons/patches/software_upgrade.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.832358 kubemarine-0.29.0/kubemarine/resources/psp/
+-rw-r--r--   0 root         (0) root         (0)      604 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/psp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/psp/anyuid.yaml
+-rw-r--r--   0 root         (0) root         (0)     1923 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/psp/default.yaml
+-rw-r--r--   0 root         (0) root         (0)     1618 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/psp/host-network.yaml
+-rw-r--r--   0 root         (0) root         (0)     1204 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/psp/privileged.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.832358 kubemarine-0.29.0/kubemarine/resources/reports/
+-rw-r--r--   0 root         (0) root         (0)      604 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/reports/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1773 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/reports/check_report.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.836358 kubemarine-0.29.0/kubemarine/resources/schemas/
+-rw-r--r--   0 root         (0) root         (0)      478 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/add_node.json
+-rw-r--r--   0 root         (0) root         (0)     2643 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/backup.json
+-rw-r--r--   0 root         (0) root         (0)     1635 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/cert_renew.json
+-rw-r--r--   0 root         (0) root         (0)      415 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/check_paas.json
+-rw-r--r--   0 root         (0) root         (0)     3317 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/cluster.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.836358 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.836358 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/common/
+-rw-r--r--   0 root         (0) root         (0)     1429 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/common/node_ref.json
+-rw-r--r--   0 root         (0) root         (0)     1722 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/common/utils.json
+-rw-r--r--   0 root         (0) root         (0)      686 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/gateway_node.json
+-rw-r--r--   0 root         (0) root         (0)     3679 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/globals.json
+-rw-r--r--   0 root         (0) root         (0)     1759 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/node.json
+-rw-r--r--   0 root         (0) root         (0)     3512 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/node_defaults.json
+-rw-r--r--   0 root         (0) root         (0)      575 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugin_defaults.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.840358 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/
+-rw-r--r--   0 root         (0) root         (0)     7227 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/calico.json
+-rw-r--r--   0 root         (0) root         (0)     2009 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/generic_plugin.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.840358 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/installation/
+-rw-r--r--   0 root         (0) root         (0)     1278 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/installation/ansible.json
+-rw-r--r--   0 root         (0) root         (0)      689 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/installation/config.json
+-rw-r--r--   0 root         (0) root         (0)     3120 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/installation/expect.json
+-rw-r--r--   0 root         (0) root         (0)     1220 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/installation/helm.json
+-rw-r--r--   0 root         (0) root         (0)      606 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/installation/python.json
+-rw-r--r--   0 root         (0) root         (0)     2265 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/installation/shell.json
+-rw-r--r--   0 root         (0) root         (0)     2498 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/installation/template.json
+-rw-r--r--   0 root         (0) root         (0)     1780 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/installation.json
+-rw-r--r--   0 root         (0) root         (0)     3129 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/kubernetes-dashboard.json
+-rw-r--r--   0 root         (0) root         (0)     1743 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/local-path-provisioner.json
+-rw-r--r--   0 root         (0) root         (0)     3472 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/nginx-ingress-controller.json
+-rw-r--r--   0 root         (0) root         (0)      605 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins.json
+-rw-r--r--   0 root         (0) root         (0)      749 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/procedures.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.844358 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/rbac/
+-rw-r--r--   0 root         (0) root         (0)      661 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/rbac/account.json
+-rw-r--r--   0 root         (0) root         (0)     3266 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/rbac/account_defaults.json
+-rw-r--r--   0 root         (0) root         (0)     3759 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/rbac/psp.json
+-rw-r--r--   0 root         (0) root         (0)     2453 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/rbac/pss.json
+-rw-r--r--   0 root         (0) root         (0)      709 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/rbac.json
+-rw-r--r--   0 root         (0) root         (0)     1951 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/registry.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.848358 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/
+-rw-r--r--   0 root         (0) root         (0)     1948 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/audit.json
+-rw-r--r--   0 root         (0) root         (0)     9668 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/coredns.json
+-rw-r--r--   0 root         (0) root         (0)     3115 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/cri.json
+-rw-r--r--   0 root         (0) root         (0)      644 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/etc_hosts.json
+-rw-r--r--   0 root         (0) root         (0)     1963 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/kernel_security.json
+-rw-r--r--   0 root         (0) root         (0)     5430 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/kubeadm.json
+-rw-r--r--   0 root         (0) root         (0)      998 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/kubeadm_kube-proxy.json
+-rw-r--r--   0 root         (0) root         (0)      938 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/kubeadm_kubelet.json
+-rw-r--r--   0 root         (0) root         (0)     2764 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/kubeadm_patches.json
+-rw-r--r--   0 root         (0) root         (0)     5264 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/loadbalancer.json
+-rw-r--r--   0 root         (0) root         (0)     1001 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/modprobe.json
+-rw-r--r--   0 root         (0) root         (0)     2302 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/ntp.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.848358 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/packages/
+-rw-r--r--   0 root         (0) root         (0)     4268 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/packages/associations.json
+-rw-r--r--   0 root         (0) root         (0)     5144 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/packages.json
+-rw-r--r--   0 root         (0) root         (0)      479 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/resolv.conf.json
+-rw-r--r--   0 root         (0) root         (0)     1243 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/sysctl.json
+-rw-r--r--   0 root         (0) root         (0)     3302 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/thirdparties.json
+-rw-r--r--   0 root         (0) root         (0)     1965 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services.json
+-rw-r--r--   0 root         (0) root         (0)     3130 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/vrrp_ip.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.848358 kubemarine-0.29.0/kubemarine/resources/schemas/internal/
+-rw-r--r--   0 root         (0) root         (0)     1343 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/internal/connections.json
+-rw-r--r--   0 root         (0) root         (0)      757 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/manage_psp.json
+-rw-r--r--   0 root         (0) root         (0)     1657 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/manage_pss.json
+-rw-r--r--   0 root         (0) root         (0)     1749 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/migrate_cri.json
+-rw-r--r--   0 root         (0) root         (0)     2885 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/migrate_kubemarine.json
+-rw-r--r--   0 root         (0) root         (0)      798 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/reboot.json
+-rw-r--r--   0 root         (0) root         (0)     2326 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/reconfigure.json
+-rw-r--r--   0 root         (0) root         (0)      872 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/remove_node.json
+-rw-r--r--   0 root         (0) root         (0)     3365 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/restore.json
+-rw-r--r--   0 root         (0) root         (0)     3504 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/upgrade.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.852358 kubemarine-0.29.0/kubemarine/resources/scripts/
+-rw-r--r--   0 root         (0) root         (0)      604 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/scripts/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      288 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/scripts/check_haproxy.sh
+-rw-r--r--   0 root         (0) root         (0)     2108 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/scripts/check_url_availability.py
+-rwxr-xr-x   0 root         (0) root         (0)     3646 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/scripts/etcdctl.sh
+-rwxr-xr-x   0 root         (0) root         (0)  2664799 2024-04-19 15:14:20.000000 kubemarine-0.29.0/kubemarine/resources/scripts/ipip_check.gz
+-rw-r--r--   0 root         (0) root         (0)     1483 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/scripts/simple_port_client.py
+-rw-r--r--   0 root         (0) root         (0)     2022 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/scripts/simple_port_listener.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.788358 kubemarine-0.29.0/kubemarine/resources/scripts/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.852358 kubemarine-0.29.0/kubemarine/resources/scripts/source/ipip_check/
+-rw-r--r--   0 root         (0) root         (0)       71 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/scripts/source/ipip_check/go.mod
+-rw-r--r--   0 root         (0) root         (0)     1446 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/scripts/source/ipip_check/go.sum
+-rw-r--r--   0 root         (0) root         (0)     5732 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/scripts/source/ipip_check/ipip_check.go
+-rw-r--r--   0 root         (0) root         (0)     8497 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/selinux.py
+-rw-r--r--   0 root         (0) root         (0)     4073 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/sysctl.py
+-rw-r--r--   0 root         (0) root         (0)    26293 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/system.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.856358 kubemarine-0.29.0/kubemarine/templates/
+-rw-r--r--   0 root         (0) root         (0)      604 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      667 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/templates/admission.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     2431 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/templates/haproxy.cfg.j2
+-rw-r--r--   0 root         (0) root         (0)      996 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/templates/keepalived.conf.j2
+-rw-r--r--   0 root         (0) root         (0)     1126 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/templates/kubelet.service.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.856358 kubemarine-0.29.0/kubemarine/templates/patches/
+-rw-r--r--   0 root         (0) root         (0)      151 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/templates/patches/control-plane-pod.json.j2
+-rw-r--r--   0 root         (0) root         (0)       76 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/templates/patches/kubelet.yaml.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.860358 kubemarine-0.29.0/kubemarine/templates/plugins/
+-rw-r--r--   0 root         (0) root         (0)      604 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/templates/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      879 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/templates/plugins/calico-ippool.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)      286 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/templates/plugins/calico-kube-controllers-metrics.yaml
+-rw-r--r--   0 root         (0) root         (0)      245 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/templates/plugins/calico-metrics.yaml
+-rw-r--r--   0 root         (0) root         (0)      436 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/templates/plugins/calico-rr.sh.j2
+-rw-r--r--   0 root         (0) root         (0)      960 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/templates/plugins/calico-rr.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)      262 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/templates/plugins/calico-typha-metrics.yaml
+-rw-r--r--   0 root         (0) root         (0)      136 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/templates/plugins/calicoctl.cfg.j2
+-rw-r--r--   0 root         (0) root         (0)      107 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/templates/plugins/dashboard-ingress.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     8826 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/templates/plugins/dashboard-v2.5.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     8905 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/templates/plugins/dashboard-v2.7.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     2749 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/templates/plugins/iperf3.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     5401 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/templates/plugins/local-path-provisioner.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     9973 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.2.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)    17847 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.4.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)    12104 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/testsuite.py
+-rw-r--r--   0 root         (0) root         (0)    19586 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/thirdparties.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/version
+-rw-r--r--   0 root         (0) root         (0)     5696 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/yum.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.860358 kubemarine-0.29.0/kubemarine.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    14049 2024-04-19 15:14:25.000000 kubemarine-0.29.0/kubemarine.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10848 2024-04-19 15:14:25.000000 kubemarine-0.29.0/kubemarine.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 15:14:25.000000 kubemarine-0.29.0/kubemarine.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2024-04-19 15:14:25.000000 kubemarine-0.29.0/kubemarine.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      516 2024-04-19 15:14:25.000000 kubemarine-0.29.0/kubemarine.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-19 15:14:25.000000 kubemarine-0.29.0/kubemarine.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5790 2024-04-19 15:14:01.000000 kubemarine-0.29.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-19 15:14:25.860358 kubemarine-0.29.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1628 2024-04-19 15:14:01.000000 kubemarine-0.29.0/setup.py
```

### Comparing `kubemarine-0.28.1/LICENSE` & `kubemarine-0.29.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/PKG-INFO` & `kubemarine-0.29.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubemarine
-Version: 0.28.1
+Version: 0.29.0
 Summary: Management tool for Kubernetes cluster deployment and maintenance
 Home-page: https://github.com/Netcracker/KubeMarine
 Author-email: Kubemarine Group <kubemarinegroup@netcracker.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Netcracker/KubeMarine
 Project-URL: Documentation, https://github.com/Netcracker/KubeMarine#documentation
 Project-URL: Issues, https://github.com/Netcracker/KubeMarine/issues/
@@ -49,50 +49,52 @@
 Requires-Dist: types-PyYAML==6.*; extra == "mypy"
 Requires-Dist: types-invoke==2.*; extra == "mypy"
 Requires-Dist: types-toml==0.*; extra == "mypy"
 Requires-Dist: types-python-dateutil==2.*; extra == "mypy"
 Requires-Dist: types-paramiko==3.*; extra == "mypy"
 Requires-Dist: types-jsonschema==4.*; extra == "mypy"
 Requires-Dist: types-pyinstaller==6.2.0.*; extra == "mypy"
+Provides-Extra: pylint
+Requires-Dist: pylint==3.1.*; extra == "pylint"
 
 ![Kubemarine_1280х640_3_JPEG](https://user-images.githubusercontent.com/5212888/162978291-63d55f19-7dc0-4126-ad39-cd69191e7e19.jpg)
 [![GitHub stars](https://img.shields.io/github/v/release/Netcracker/Kubemarine)](https://github.com/Netcracker/KubeMarine/releases)
 [![GitHub stars](https://img.shields.io/badge/contributions-welcome-orange.svg)](https://github.com/Netcracker/KubeMarine/blob/main/CONTRIBUTING.md)
 [![PyPI version](https://badge.fury.io/py/kubemarine.svg)](https://badge.fury.io/py/kubemarine)
 
 # Kubemarine
 
 Kubemarine is an open source, lightweight and powerful management tool built for end-to-end Kubernetes cluster deployment and maintenance. It is applicable for many purposes like simple and quick onboarding Kubernetes on local and production environments in different HA schemes depending on your aims, budget, and capabilities. Together with simplicity, Kubemarine can be a very flexible and customizable tool covering specific configurability cases on both deployment and maintenance stages. This library provides powerful CLI commands, as well as can be customized using a Python extension API.
 
 ## Highlights
 - Easy to use
-- Many procedures supported following the [generic maintenance approach](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#basics):
-  - [install](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#)
-  - [add_node](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#add-node-procedure)
-  - [remove_node](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#remove-node-procedure)
-  - [upgrade](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#upgrade-procedure)
-  - [backup](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#backup-procedure)
-  - [restore](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#restore-procedure)
-  - [reconfigure](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#reconfigure-procedure)
-  - [check_iaas](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Kubecheck.md#iaas-procedure)
-  - [check_paas](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Kubecheck.md#paas-procedure)
-  - [migrate_kubemarine](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#kubemarine-migration-procedure)
-  - [manage_psp](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#manage-psp-procedure)
-  - [manage_pss](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#manage-pss-procedure)
-  - [cert_renew](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#certificate-renew-procedure)
-  - [migrate_cri](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#cri-migration-procedure)
-- [Single cluster inventory](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#configuration) for all operations, highly customizable
+- Many procedures supported following the [generic maintenance approach](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#basics):
+  - [install](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#)
+  - [add_node](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#add-node-procedure)
+  - [remove_node](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#remove-node-procedure)
+  - [upgrade](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#upgrade-procedure)
+  - [backup](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#backup-procedure)
+  - [restore](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#restore-procedure)
+  - [reconfigure](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#reconfigure-procedure)
+  - [check_iaas](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Kubecheck.md#iaas-procedure)
+  - [check_paas](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Kubecheck.md#paas-procedure)
+  - [migrate_kubemarine](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#kubemarine-migration-procedure)
+  - [manage_psp](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#manage-psp-procedure)
+  - [manage_pss](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#manage-pss-procedure)
+  - [cert_renew](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#certificate-renew-procedure)
+  - [migrate_cri](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#cri-migration-procedure)
+- [Single cluster inventory](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#configuration) for all operations, highly customizable
 - Default values of all parameters in configurations with a minimum of required parameters
-- [Control planes balancing](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#full-ha-scheme) with external balancers and VRRP
-- Ability to [resume or skip specific task](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#tasks-list-redefinition) without re-running entire pipeline
-- [Pre-built plugins](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#predefined-plugins) out of the box and [custom plugins](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#custom-plugins-installation-procedures) support
-- Support for [executing in closed environments](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#installation-without-internet-resources) with private registries
-- Extended [logging](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Logging.md), configs [dumping](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#dump-files)
+- [Control planes balancing](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#full-ha-scheme) with external balancers and VRRP
+- Ability to [resume or skip specific task](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#tasks-list-redefinition) without re-running entire pipeline
+- [Pre-built plugins](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#predefined-plugins) out of the box and [custom plugins](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#custom-plugins-installation-procedures) support
+- Support for [executing in closed environments](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#installation-without-internet-resources) with private registries
+- Extended [logging](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Logging.md), configs [dumping](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#dump-files)
 - Build supported as a package, container, and binary
-- Package extension with [open extension API](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/PackageExtension.md)
+- Package extension with [open extension API](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/PackageExtension.md)
 - Support different deployment schemes (all-in-one, mini-HA, HA, and so on)
 
 ## Kubemarine Binary Installation
 Proceed the following steps to install Kubemarine  on your environment:
 1. Download the binary file for your system from the latest [release](https://github.com/Netcracker/KubeMarine/releases)
 2. Move binary kubemarine to a separate folder 
 3. Now you can proceed to run Kubemarine! Try the following:
@@ -110,15 +112,15 @@
    ```bash
    python3 -m pip install --upgrade pip
    ```
    Windows:
    ```bash
    python -m pip install --upgrade pip
    ```
-1. Ensure your environment meets the [Deployment Node Prerequisites](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#prerequisites-for-deployment-node).
+1. Ensure your environment meets the [Deployment Node Prerequisites](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#prerequisites-for-deployment-node).
 1. Create and activate a [virtual environment](https://realpython.com/python-virtual-environments-a-primer/) if necessary.
 1. Install Kubemarine package.
 
    Linux / MacOS:
    ```bash
    python3 -m pip install kubemarine
    ```
@@ -129,15 +131,15 @@
 1. Now you can proceed to run Kubemarine! Try the following:
    ```bash
    kubemarine help
    ```
 
 
 ## Kubemarine Installation from Sources
-Installation of Kubemarine from sources is mostly similar to [Kubemarine Package Installation](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/README.md#kubemarine-package-installation).
+Installation of Kubemarine from sources is mostly similar to [Kubemarine Package Installation](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/README.md#kubemarine-package-installation).
 The exception is instead of installing the package from [PyPI](https://pypi.org/project/kubemarine/), do the following:
 1. [Download the latest release](https://github.com/netcracker/kubemarine/releases) or clone the repository:
    ```bash
    git clone https://github.com/netcracker/kubemarine.git
    ```
 1. Unpack the project from the archive if required:
    ```bash
@@ -158,24 +160,24 @@
    python -m pip install -e .
    ```
 1. Now you can proceed to run Kubemarine. Try the following:
     ```bash
     kubemarine help
     ```
 
-**Note**: Building from [Dockerfile](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/Dockerfile) is also available.
+**Note**: Building from [Dockerfile](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/Dockerfile) is also available.
 
 
 **Note:** Kubemarine debugging available via `kubemarine/__main__.py`.
 
 
 ## Running Cluster Installation
 To install a Kubernetes cluster using Kubemarine:
-1. Prepare your VMs or bare-metal machines according to [Recommended Hardware Requirements](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#recommended-hardware-requirements) and the selected [Deployment Scheme](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#deployment-schemes). Make sure the nodes meet [Cluster Nodes Prerequisites](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#prerequisites-for-cluster-nodes).
-1. Create the `cluster.yaml` inventory file, and describe your environment. Make sure that all configurations are done. For more information, see [inventory configs available](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#configuration) and [examples](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/examples/cluster.yaml). No need to enter all the parameters that are available, it is enough to specify the minimal identification data about the nodes where you want to install the cluster, for example:
+1. Prepare your VMs or bare-metal machines according to [Recommended Hardware Requirements](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#recommended-hardware-requirements) and the selected [Deployment Scheme](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#deployment-schemes). Make sure the nodes meet [Cluster Nodes Prerequisites](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#prerequisites-for-cluster-nodes).
+1. Create the `cluster.yaml` inventory file, and describe your environment. Make sure that all configurations are done. For more information, see [inventory configs available](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#configuration) and [examples](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/examples/cluster.yaml). No need to enter all the parameters that are available, it is enough to specify the minimal identification data about the nodes where you want to install the cluster, for example:
    ```yaml
    node_defaults:
      keyfile: "/home/username/.ssh/id_rsa"
      password: '{{ env.PASS }}'     #Either keyfile or password can be used.
      username: "centos"
 
    vrrp_ips:
@@ -204,42 +206,42 @@
    kubemarine install
    ```
 1. Check the health of the newly installed cluster:
    ```bash
    kubemarine check_paas
    ```
 
-For more information, refer to the other [Kubemarine guides](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/README.md#documentation).
+For more information, refer to the other [Kubemarine guides](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/README.md#documentation).
 
 ## Kubemarine Docker Installation
 To start, download the Kubmarine image ```docker pull ghcr.io/netcracker/kubemarine:main```
 
 Run Kubemarine from the container, for example:
    ```
    docker run -it --mount type=bind,source=/root/cluster.yaml,target=/opt/kubemarine/cluster.yaml --mount type=bind,source=/root/rsa_key,target=/opt/kubemarine/rsa_key kubemarine install -c /opt/kubemarine/cluster.yaml
    ```
    *Note*: Do not forget to pass the inventory file and connection key inside the container.
    For more execution details, refer to ["Installation of Kubernetes using CLI" guide on Github](https://github.com/Netcracker/kubemarine/blob/main/documentation/Installation.md#installation-of-kubernetes-using-cli).
 
 ## Documentation
 The following documents and tutorials are available:
-- [Installation](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md)
-- [Maintenance](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md)
-- [Troubleshooting](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Troubleshooting.md)
-- [Kubecheck](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Kubecheck.md)
-- [Logging](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Logging.md)
+- [Installation](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md)
+- [Maintenance](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md)
+- [Troubleshooting](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Troubleshooting.md)
+- [Kubecheck](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Kubecheck.md)
+- [Logging](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Logging.md)
 
 Also, check out the following inventory examples:
-- [cluster.yaml](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/examples/cluster.yaml)
-- [procedure.yaml](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/examples/procedure.yaml)
+- [cluster.yaml](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/examples/cluster.yaml)
+- [procedure.yaml](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/examples/procedure.yaml)
 
 ## Issues, Questions
 If you have any problems while working with Kubemarine, feel free to open a [new issue](https://github.com/netcracker/kubemarine/issues) or even
 [PR](https://github.com/netcracker/kubemarine/pulls) with related changes.
-Please follow the [Contribution Guide](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/CONTRIBUTING.md ) and the process outlined in the Stack Overflow [MCVE](https://stackoverflow.com/help/mcve) document.
+Please follow the [Contribution Guide](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/CONTRIBUTING.md ) and the process outlined in the Stack Overflow [MCVE](https://stackoverflow.com/help/mcve) document.
 
-In case of security concerns, please follow the [Security Reporting Process](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/SECURITY.md)
+In case of security concerns, please follow the [Security Reporting Process](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/SECURITY.md)
 ## Changelog
 Detailed changes for each release are documented in the [release notes](https://github.com/netcracker/kubemarine/releases).
 
 ## License
-[Apache License 2.0](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/LICENSE)
+[Apache License 2.0](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/LICENSE)
```

### Comparing `kubemarine-0.28.1/README.md` & `kubemarine-0.29.0/README.md`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/bin/kubemarine` & `kubemarine-0.29.0/bin/kubemarine`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/bin/kubemarine.cmd` & `kubemarine-0.29.0/bin/kubemarine.cmd`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/__init__.py` & `kubemarine-0.29.0/kubemarine/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/__main__.py` & `kubemarine-0.29.0/kubemarine/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,24 +21,26 @@
 from typing import Dict, List
 
 import ruamel.yaml.resolver
 import yaml
 
 from kubemarine import procedures as proc
 
+# pylint: disable=bad-builtin
+
 # Don't remove this line. The idna encoding
 # is used by getaddrinfo when dealing with unicode hostnames,
 # and in some cases, there appears to be a race condition
 # where threads will get a LookupError on getaddrinfo() saying
 # that the encoding doesn't exist.  Using the idna encoding before
 # running any kubemarine code (and any threads it may create) ensures that
 # the encodings.idna is imported and registered in the codecs registry,
 # which will stop the LookupErrors from happening.
 # See: https://bugs.python.org/issue29288
-u''.encode('idna')
+u''.encode('idna')  # pylint: disable=redundant-u-string-prefix
 
 # Take pattern to resolve float used by ruamel instead of that is used by pyyaml.
 # https://sourceforge.net/p/ruamel-yaml/code/ci/0.17.21/tree/resolver.py#l43
 # Initially introduced for keepalived that generates random password string.
 # The generated string might be also a valid exponential float, and should be dumped with quotes.
 # See also:
 # https://stackoverflow.com/questions/30458977/yaml-loads-5e-6-as-string-and-not-a-number
@@ -181,15 +183,15 @@
 
 
 def selftest() -> None:
     print("Running selftest")
 
     time_start = int(round(time.time() * 1000))
 
-    for procedure, procedure_details in procedures.items():
+    for procedure in procedures:
         print("\nImporting %s..." % procedure)
 
         if procedure in ['version', 'selftest']:
             continue
 
         module = proc.import_procedure(procedure)
         imports = []
```

### Comparing `kubemarine-0.28.1/kubemarine/admission.py` & `kubemarine-0.29.0/kubemarine/admission.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,21 +11,20 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import io
 import os
 import re
-from typing import Dict, Any, List, Optional, Union
+from typing import Dict, List, Optional, Union
 
 import ruamel.yaml
 import yaml
 from jinja2 import Template
 
-from kubemarine import kubernetes
 from kubemarine.core import utils
 from kubemarine.core.cluster import KubernetesCluster, EnrichmentStage, enrichment
 from kubemarine.core.group import NodeGroup, RunnersGroupResult
 from kubemarine.core.yaml_merger import default_merger
 from kubemarine.kubernetes import components
 from kubemarine.plugins import builtin
 
@@ -41,16 +40,14 @@
 bindings_list_option = "bindings-list"
 
 provided_oob_policies = ["default", "host-network", "anyuid"]
 
 valid_modes = ['enforce', 'audit', 'warn']
 valid_versions_templ = r"^v1\.\d{1,2}$"
 
-loaded_oob_policies = {}
-
 ERROR_INCONSISTENT_INVENTORIES = "Procedure config and cluster config are inconsistent. Please check 'admission' option"
 ERROR_CHANGE_OOB_PSP_DISABLED = "OOB policies can not be configured when security is disabled"
 ERROR_PSS_BOTH_STATES_DISABLED = ("both 'pod-security' in procedure config and current config are 'disabled'. "
                                   "There is nothing to change")
 
 # TODO: When KubeMarine is not support Kubernetes version lower than 1.25, the PSP implementation code should be deleted 
 
@@ -63,17 +60,14 @@
     return components.kubernetes_minor_release_at_least(cluster.inventory, "v1.28")
 
 
 @enrichment(EnrichmentStage.FULL)
 def enrich_inventory_psp(cluster: KubernetesCluster) -> None:
     inventory = cluster.inventory
 
-    global loaded_oob_policies
-    loaded_oob_policies = load_oob_policies_files()
-
     # validate custom
     custom_policies = inventory["rbac"]["psp"]["custom-policies"]
     verify_custom(custom_policies)
 
     # do not perform enrichment if security disabled
     if not is_security_enabled(inventory):
         return
@@ -161,19 +155,19 @@
         verify_custom_list(roles_list, "role")
 
     bindings_list = custom_scope.get(bindings_list_option, None)
     if bindings_list:
         verify_custom_list(bindings_list, "binding")
 
 
-def verify_custom_list(custom_list: List[dict], type: str) -> None:
+def verify_custom_list(custom_list: List[dict], type_: str) -> None:
     for item in custom_list:
         # forbid using 'oob-' prefix in order to avoid conflicts of our policies and users policies
         if item["metadata"]["name"].startswith("oob-"):
-            raise Exception("Name %s is not allowed for custom %s" % (item["metadata"]["name"], type))
+            raise Exception("Name %s is not allowed for custom %s" % (item["metadata"]["name"], type_))
 
 
 def verify_version(owner: str, version: str, kubernetes_version: str) -> None:
     # check Kubernetes version and admission config matching
     if version != "latest":
         result = re.match(valid_versions_templ, version)
         if result is None:
@@ -298,15 +292,17 @@
         cluster.log.debug("No need to reconfigure OOB policies, skipping...")
         return
 
     first_control_plane = cluster.nodes["control-plane"].get_first_member()
 
     cluster.log.debug("Deleting all OOB policies...")
     first_control_plane.call(delete_privileged_policy)
-    first_control_plane.call(manage_policies, manage_type="delete", manage_scope=resolve_oob_scope(loaded_oob_policies, "all"))
+    first_control_plane.call(manage_policies,
+                             manage_type="delete",
+                             manage_scope=resolve_oob_scope(target_config, "all"))
 
     if target_state == "disabled":
         cluster.log.debug("Security disabled, OOB will not be recreated")
         return
 
     cluster.log.debug("Recreating all OOB policies...")
     first_control_plane.call(apply_privileged_policy)
@@ -323,14 +319,16 @@
         cluster.log.debug("Security plugin will not be reconfigured")
         return
 
     cluster.nodes['control-plane'].call(components.reconfigure_components, components=['kube-apiserver'])
 
 
 def restart_pods_task(cluster: KubernetesCluster) -> None:
+    from kubemarine import kubernetes  # pylint: disable=cyclic-import
+
     if cluster.context.get('initial_procedure') == 'manage_pss':
         # check if pods restart is enabled
         is_restart = cluster.procedure_inventory.get("restart-pods", False)
         if not is_restart:
             cluster.log.debug("'restart-pods' is disabled, pods won't be restarted")
             return
 
@@ -385,23 +383,25 @@
     privileged_policy = utils.read_internal(os.path.join(policies_file_path, filename))
     remote_path = utils.get_remote_tmp_path(filename)
     group.put(io.StringIO(privileged_policy), remote_path, backup=True, sudo=True)
 
     return group.sudo("kubectl %s -f %s" % (manage_type, remote_path), warn=True)
 
 
-def resolve_oob_scope(oob_policies_conf: Dict[str, Any], selector: str) -> Dict[str, List[dict]]:
+def resolve_oob_scope(oob_policies_conf: Dict[str, str], selector: str) -> Dict[str, List[dict]]:
     result: Dict[str, List[dict]] = {
         psp_list_option: [],
         roles_list_option: [],
         bindings_list_option: []
     }
 
+    loaded_oob_policies = load_oob_policies_files()
+
     for key, value in oob_policies_conf.items():
-        if value == selector or selector == "all":
+        if selector in (value, "all"):
             policy = loaded_oob_policies[key]
             if "psp" in policy:
                 result[psp_list_option].append(policy["psp"])
             if "role" in policy:
                 result[roles_list_option].append(policy["role"])
             if "binding" in policy:
                 result[bindings_list_option].append(policy["binding"])
@@ -436,16 +436,14 @@
     group.sudo("rm -f %s" % remote_path)
     return result
 
 
 def collect_policies_template(psp_list: Optional[List[dict]],
                               roles_list: Optional[List[dict]],
                               bindings_list: Optional[List[dict]]) -> str:
-    yaml = ruamel.yaml.YAML()
-
     buf = io.StringIO()
     if psp_list:
         for psp in psp_list:
             yaml.dump(psp, buf)
             buf.write("\n---\n")
     if roles_list:
         for role in roles_list:
@@ -473,19 +471,18 @@
             and cluster.inventory["rbac"]["pss"]["pod-security"] == "disabled"):
         raise Exception(ERROR_PSS_BOTH_STATES_DISABLED)
 
     if "namespaces" in procedure_config:
         for namespace_item in procedure_config["namespaces"]:
             # check if the namespace has its own profiles
             if isinstance(namespace_item, dict):
-                namespace = list(namespace_item.keys())[0]
-                for item in list(namespace_item[namespace]):
-                    if namespace_item[namespace][item]:
-                        if item.endswith("version"):
-                            verify_version(item, namespace_item[namespace][item], kubernetes_version)
+                profiles = list(namespace_item.values())[0]
+                for item in profiles:
+                    if item.endswith("version"):
+                        verify_version(item, profiles[item], kubernetes_version)
     if "namespaces_defaults" in procedure_config:
         for item in procedure_config["namespaces_defaults"]:
             if item.endswith("version"):
                 verify_version(item, procedure_config["namespaces_defaults"][item], kubernetes_version)
 
 
 @enrichment(EnrichmentStage.PROCEDURE, procedures=['manage_psp', 'manage_pss'])
@@ -520,15 +517,15 @@
 
     # Admission configuration may change.
     # Force kube-apiserver pod restart, then wait for API server to become available.
     force_restart = True
 
     # Extra args of API may change, need to reconfigure the API server.
     # See enrich_inventory_pss()
-    control_planes.call(kubernetes.components.reconfigure_components,
+    control_planes.call(components.reconfigure_components,
                         components=['kube-apiserver'], force_restart=force_restart)
 
     if target_state == 'disabled':
         # erase PSS admission config
         cluster.log.debug("Erase admission configuration... %s" % admission_path)
         control_planes.sudo("rm -f %s" % admission_path, warn=True)
 
@@ -610,28 +607,28 @@
     # get the list of namespaces that should be labeled then set/delete labels
     if namespaces:
         default_modes = {}
         # check if procedure config has default values for labels
         namespaces_defaults = procedure_config.get("namespaces_defaults")
         if namespaces_defaults:
             for default_mode in namespaces_defaults:
-                 default_modes[default_mode] = namespaces_defaults[default_mode]
+                default_modes[default_mode] = namespaces_defaults[default_mode]
         for namespace in namespaces:
             # define name of namespace
             if isinstance(namespace, dict):
                 ns_name = list(namespace.keys())[0]
             else:
                 ns_name = namespace
             if security_enabled:
                 if default_modes:
                     # set labels that are set in default section
                     cluster.log.debug(f"Set PSS labels on {ns_name} namespace from defaults")
-                    for mode in default_modes:
+                    for mode, value in default_modes.items():
                         first_control_plane.sudo(f"kubectl label ns {ns_name} "
-                                f"pod-security.kubernetes.io/{mode}={default_modes[mode]} --overwrite")
+                                f"pod-security.kubernetes.io/{mode}={value} --overwrite")
                 if isinstance(namespace, dict):
                     # set labels that are set in namespaces section
                     cluster.log.debug(f"Set PSS labels on {ns_name} namespace")
                     for item in list(namespace[ns_name]):
                         first_control_plane.sudo(f"kubectl label ns {ns_name} " 
                                     f"pod-security.kubernetes.io/{item}={namespace[ns_name][item]} --overwrite")
             else:
```

### Comparing `kubemarine-0.28.1/kubemarine/apparmor.py` & `kubemarine-0.29.0/kubemarine/apparmor.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,84 +9,76 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
-from typing import Dict
+from typing import Dict, List
 
-from kubemarine import system
 from kubemarine.core import log
 from kubemarine.core.group import NodeGroup, RunnersGroupResult
 
 
-def get_status(group: NodeGroup) -> Dict[str, dict]:
+def get_status(group: NodeGroup) -> Dict[str, Dict[str, List[str]]]:
     log = group.cluster.log
     result = group.sudo("apparmor_status --json")
     parsed_result = {}
-    if result:
-        for host, node_result in result.items():
-            log.verbose('Parsing status for %s...' % host)
-            parsed_result[host] = parse_status(log, node_result.stdout)
+    for host, node_result in result.items():
+        log.verbose('Parsing status for %s...' % host)
+        parsed_result[host] = parse_status(log, node_result.stdout)
     print_status(log, parsed_result)
     return parsed_result
 
 
-def parse_status(logger: log.EnhancedLogger, result_stdout: str) -> dict:
-    result = {}
+def parse_status(logger: log.EnhancedLogger, result_stdout: str) -> Dict[str, List[str]]:
+    result: Dict[str, List[str]] = {}
     # Temporary workaround as long as we support OS with AppArmor from 3.0.0 to 3.0.8
     # Ubuntu 22.04.1 has 3.0.4
     # Malformed output is caused by false start `], ` delimiter
     # https://gitlab.com/apparmor/apparmor/-/blob/v3.0.4/binutils/aa_status.c#L537
     # https://gitlab.com/apparmor/apparmor/-/issues/295
     if '"processes": {], ' in result_stdout:
         logger.debug("Patching malformed apparmor_status --json output")
         result_stdout = result_stdout.replace('"processes": {], ', '"processes": {')
+
     parsed_data = json.loads(result_stdout)
-    modes_set = set()
-    for mode in parsed_data['profiles'].values():
-        modes_set.add(mode)
-    for mode in modes_set:
-        profile_list = []
-        for profile_name, profile_state in parsed_data['profiles'].items():
-            if profile_state == mode:
-                profile_list.append(profile_name)
-        result[profile_state] = profile_list
+    for profile_name, profile_state in parsed_data['profiles'].items():
+        result.setdefault(profile_state, []).append(profile_name)
+
     return result
 
 
 def print_status(logger: log.EnhancedLogger, parsed_result: dict) -> None:
     res = "AppArmor Status:"
     for state in parsed_result.keys():
         res += "\n  Profiles in %s mode:" % state
         for profile in parsed_result[state]:
             res += "\n    - %s" % profile
     logger.verbose(res)
 
 
-def is_state_valid(group: NodeGroup, expected_profiles: dict) -> bool:
+def is_state_valid(group: NodeGroup, expected_profiles: Dict[str, List[str]]) -> bool:
     log = group.cluster.log
 
     log.verbose('Verifying Apparmor modes...')
 
     parsed_result = get_status(group)
     valid = True
 
     for host, status in parsed_result.items():
         for state, profiles in expected_profiles.items():
             if not profiles:
                 continue
             if state == 'disable':
                 for profile in profiles:
-                    for remote_profiles in status.values():
-                        if profile in remote_profiles:
-                            valid = False
-                            log.verbose('Mode %s is enabled on remote host %s' % (state, host))
-                            break
+                    if any(profile in remote_profiles for remote_profiles in status.values()):
+                        valid = False
+                        log.verbose('Mode %s is enabled on remote host %s' % (state, host))
+                        break
             else:
                 if not status.get(state):
                     valid = False
                     log.verbose('Mode %s is not presented on remote host %s' % (state, host))
                     break
                 # check if all 'cluster.yaml' settings reflect on particular node
                 for profile in profiles:
@@ -106,26 +98,31 @@
     return profile
 
 
 def configure_apparmor(group: NodeGroup, expected_profiles: dict) -> RunnersGroupResult:
     cmd = ''
     for profile in expected_profiles.get('enforce', []):
         profile = convert_profile(profile)
-        cmd += 'sudo rm -f /etc/apparmor.d/disable/%s; sudo rm -f /etc/apparmor.d/force-complain/%s; ' % (profile, profile)
+        cmd += (f'sudo rm -f /etc/apparmor.d/disable/{profile}; '
+                f'sudo rm -f /etc/apparmor.d/force-complain/{profile}; ')
     for profile in expected_profiles.get('complain', []):
         profile = convert_profile(profile)
-        cmd += 'sudo rm -f /etc/apparmor.d/disable/%s; sudo ln -s /etc/apparmor.d/%s /etc/apparmor.d/force-complain/; ' % (profile, profile)
+        cmd += (f'sudo rm -f /etc/apparmor.d/disable/{profile}; '
+                f'sudo ln -s /etc/apparmor.d/{profile} /etc/apparmor.d/force-complain/; ')
     for profile in expected_profiles.get('disable', []):
         profile = convert_profile(profile)
-        cmd += 'sudo rm -f /etc/apparmor.d/force-complain/%s; sudo ln -s /etc/apparmor.d/%s /etc/apparmor.d/disable/; ' % (profile, profile)
+        cmd += (f'sudo rm -f /etc/apparmor.d/force-complain/{profile}; '
+                f'sudo ln -s /etc/apparmor.d/{profile} /etc/apparmor.d/disable/; ')
     cmd += 'sudo systemctl reload apparmor.service && sudo apparmor_status'
     return group.sudo(cmd)
 
 
 def setup_apparmor(group: NodeGroup) -> None:
+    from kubemarine import system  # pylint: disable=cyclic-import
+
     log = group.cluster.log
 
     if group.get_nodes_os() != 'debian':
         log.debug("Skipped - Apparmor is supported only on Ubuntu/Debian")
         return
 
     expected_profiles = group.cluster.inventory['services']['kernel_security'].get('apparmor', {})
```

### Comparing `kubemarine-0.28.1/kubemarine/apt.py` & `kubemarine-0.29.0/kubemarine/apt.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/audit.py` & `kubemarine-0.29.0/kubemarine/audit.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/controlplane.py` & `kubemarine-0.29.0/kubemarine/controlplane.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/core/__init__.py` & `kubemarine-0.29.0/kubemarine/core/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/core/action.py` & `kubemarine-0.29.0/kubemarine/core/action.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         :param recreate_inventory: Specifies if inventory should be recreated after the action succeeds.
         """
 
         self.identifier = identifier
         self.recreate_inventory = recreate_inventory
 
     @abstractmethod
-    def run(self, res: DynamicResources) -> None:
+    def run(self, _res: DynamicResources) -> None:
         """
         Do some work based on provided DynamicResources. If any action fails, further actions are not run.
 
         Avoid direct exiting in case of exceptions (for example using utils.do_fail),
         unless it is the only action being executed.
         Otherwise, correct exception handling will not be performed.
         """
@@ -46,8 +46,8 @@
     def prepare_context(self, context: dict) -> None:
         """
         Enrich context if necessary before the action is run.
         The changes are remained after action is executed, and will be visible to further actions.
 
         :param context: mutable context instance.
         """
-        return
+        pass
```

### Comparing `kubemarine-0.28.1/kubemarine/core/annotations.py` & `kubemarine-0.29.0/kubemarine/core/annotations.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/core/cluster.py` & `kubemarine-0.29.0/kubemarine/core/cluster.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,23 +8,25 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import dataclasses
+import functools
 from copy import deepcopy
 from enum import Flag, auto, IntFlag
 from types import FunctionType
 from typing import Dict, List, Union, Iterable, Tuple, Optional, Any, Callable, cast, Sequence
 
 from ordered_set import OrderedSet
 from typing_extensions import Protocol
 
-from kubemarine.core import log, utils, static
+from kubemarine.core import log  # pylint: disable=unused-import
+from kubemarine.core import utils, static
 from kubemarine.core.connections import ConnectionPool
 from kubemarine.core.environment import Environment
 from kubemarine.core.errors import KME0006
 from kubemarine.core.group import NodeGroup, NodeConfig
 
 _AnyConnectionTypes = Union[str, NodeGroup]
 
@@ -130,15 +132,15 @@
     """
     Wraps callable that performs enrichment, persisting selectors as the wrapper attributes.
     The selectors are supplied as the arguments of this decorator.
 
     :param stages: `EnrichmentStage` stages to run this function at.
     :param procedures: list of procedures for which the function is applicable.
     """
-    return lambda fn: EnrichmentFunction(fn, stages, procedures)
+    return lambda fn: functools.wraps(fn)(EnrichmentFunction(fn, stages, procedures))
 
 
 @dataclasses.dataclass(repr=False)
 class _EnrichmentProducts:
     """States of inventory and context at the particular `EnrichmentStage` of enrichment."""
     inventory: dict
     context: Optional[dict]
@@ -188,16 +190,18 @@
 
         # Flag.name is not None for not compound values in any Python version.
         self.log.verbose(f"Starting {cast(str, stage.name).lower()!r} enrichment")
 
         self._enrichment_stage = stage
         if stage == EnrichmentStage.DEFAULT:
             self._products.procedure_inventory = None
+            args: dict = self.context['execution_arguments']
+            args.pop('procedure_config', None)
         if stage == EnrichmentStage.PROCEDURE and previous_cluster is not None:
-            self._previous_products = previous_cluster._products
+            self._previous_products = previous_cluster._products  # pylint: disable=protected-access
 
             # Previous nodes refer to previous cluster. Create new group to surely refer to this cluster.
             self._products.nodes['previous'] = {
                 role: self.make_group(group.nodes)
                 for role, group in self._previous_products.nodes['nodes'].items()}
 
         if stage == EnrichmentStage.LIGHT:
@@ -223,17 +227,23 @@
         self.log.verbose('Enrichment finished!')
 
         return self
 
     @enrichment(EnrichmentStage.ALL)
     def convert_formatted_inventory(self) -> dict:
         products = self._products
-        products.formatted_inventory = self.inventory
+        if self._enrichment_stage != EnrichmentStage.LIGHT:
+            products.formatted_inventory = self.inventory
+
         products.raw_inventory = utils.convert_native_yaml(self.inventory)
-        if products.procedure_inventory is not None:
+
+        if self._enrichment_stage == EnrichmentStage.LIGHT:
+            # inventory['nodes'] is already enriched, and the procedure inventory is no longer necessary.
+            products.procedure_inventory = None
+        elif self._enrichment_stage == EnrichmentStage.PROCEDURE:
             products.procedure_inventory = utils.convert_native_yaml(self.procedure_inventory)
 
         return utils.deepcopy_yaml(products.raw_inventory)
 
     @enrichment(EnrichmentStage.LIGHT)
     def init_nodes_context(self) -> None:
         self._connection_pool = self.create_connection_pool(self._get_all_nodes().get_hosts())
@@ -250,17 +260,17 @@
                 ('add_node', self.get_new_nodes()),
                 ('remove_node', self.get_nodes_for_removal()),
         ):
             if not group.is_empty():
                 ips[role] = OrderedSet(group.get_hosts())
 
         self.log.debug("Inventory file loaded:")
-        for role in ips.keys():
-            self.log.debug("  %s %i" % (role, len(ips[role])))
-            for ip in ips[role]:
+        for role, hosts in ips.items():
+            self.log.debug("  %s %i" % (role, len(hosts)))
+            for ip in hosts:
                 self.log.debug("    %s" % ip)
 
     @property
     def previous_nodes(self) -> Dict[str, NodeGroup]:
         """
         Previous nodes of the cluster.
         For the cluster enriched at PROCEDURE stage, this includes nodes to be removed, but does not include added nodes.
@@ -311,15 +321,15 @@
 
         return context
 
     @property
     def procedure_inventory(self) -> dict:
         procedure_inventory = self._products.procedure_inventory
         if procedure_inventory is None:
-            raise ValueError("Procedure inventory is not available at 'default' enrichment stage")
+            raise ValueError("Procedure inventory is not available at 'default' or 'light' enrichment stage")
 
         return procedure_inventory
 
     @property
     def previous_raw_inventory(self) -> dict:
         """
         Inventory represented in python native objects before applying of any enrichment.
@@ -356,15 +366,15 @@
         for maintenance procedures that have specific enrichment functions,
         and that support inventory recreation.
 
         The property should be read only.
         """
         formatted_inventory = self._products.formatted_inventory
         if formatted_inventory is None:
-            raise ValueError("Enrichment is not yet started")
+            raise ValueError("Formatted inventory is not available at 'light' enrichment stage")
 
         return formatted_inventory
 
     @property
     def nodes_context(self) -> Dict[str, Any]:
         """Various information about nodes that is not changed during Kubemarine run."""
         if self._nodes_context is None:
@@ -481,34 +491,62 @@
 
         if nodes_names:
             common_group = common_group.include_group(self.make_group_from_nodes(nodes_names))
 
         return common_group
 
     def schedule_cumulative_point(self, point_method: Callable) -> None:
-        from kubemarine.core import flow
-        flow.schedule_cumulative_point(self, point_method)
+        self._check_within_flow()
+
+        func = cast(FunctionType, point_method)
+        point_fullname = func.__module__ + '.' + func.__qualname__
+
+        if self.context['execution_arguments'].get('disable_cumulative_points', False):
+            self.log.verbose('Method %s not scheduled - cumulative points disabled' % point_fullname)
+            return
+
+        if point_fullname in self.context['execution_arguments']['exclude_cumulative_points_methods']:
+            self.log.verbose('Method %s not scheduled - it set to be excluded' % point_fullname)
+            return
+
+        scheduled_points = self.context.get('scheduled_cumulative_points', [])
+
+        if point_method not in scheduled_points:
+            scheduled_points.append(point_method)
+            self.context['scheduled_cumulative_points'] = scheduled_points
+            self.log.verbose('Method %s scheduled' % point_fullname)
+        else:
+            self.log.verbose('Method %s already scheduled' % point_fullname)
 
     def is_task_completed(self, task_path: str) -> bool:
-        from kubemarine.core import flow
-        return flow.is_task_completed(self, task_path)
+        self._check_within_flow()
+        return task_path in self.context['proceeded_tasks']
+
+    def _check_within_flow(self, check: bool = True) -> None:
+        if check != ('proceeded_tasks' in self.context):
+            raise NotImplementedError(f"The method is called {'not ' if check else ''}within tasks flow execution")
 
     def check_nodes_accessibility(self, skip_check_iaas: bool = True) -> None:
         """Check nodes access statuses"""
 
         procedure: str = self.context['initial_procedure']
         if procedure == 'check_iaas' and skip_check_iaas:
             return
+        
+        if procedure == 'remove_node':
+            group = self.make_group_from_roles(['control-plane', 'balancer'])
+        else:
+            group = self.make_group_from_roles(['control-plane', 'balancer']).include_group(self.get_new_nodes_or_self())
 
-        # Check that only subset of nodes for removal can be offline
-        remained_offline = self.nodes['all'].get_online_nodes(False)
+        # Check that nodes are online
+        remained_offline = group.get_online_nodes(False)
 
-        # Check that all online nodes are accessible.
-        all_nodes = self._get_all_nodes()
-        inaccessible_online = all_nodes.get_online_nodes(True).exclude_group(all_nodes.get_accessible_nodes())
+        # Check that nodes are accessible.
+        nodes = group.include_group(self.get_changed_nodes())
+        inaccessible_online = nodes.get_online_nodes(True).exclude_group(nodes.get_accessible_nodes())
 
         if not remained_offline.is_empty() or not inaccessible_online.is_empty():
             raise KME0006(remained_offline.get_hosts(), inaccessible_online.get_hosts())
 
     def get_os_family_for_node(self, host: str) -> str:
         os_family: Optional[str] = self.nodes_context.get(host, {}).get('os', {}).get('family')
         if os_family is None:
@@ -648,16 +686,16 @@
             -> dict:
         prepared_inventory = utils.deepcopy_yaml(self.inventory)
         for finalize_fn in finalization_functions:
             prepared_inventory = finalize_fn(self, prepared_inventory)
 
         return prepared_inventory
 
-    def preserve_inventory(self, context: dict) -> None:
+    def preserve_inventory(self, context: dict, *, enriched: bool = True) -> None:
         self.log.debug("Start preserving of the information about the procedure.")
         cluster_storage = self._create_cluster_storage(context)
         cluster_storage.make_dir()
         if self.context.get('initial_procedure') == 'add_node':
             cluster_storage.upload_info_new_control_planes()
         cluster_storage.collect_procedure_info()
-        cluster_storage.compress_archive()
+        cluster_storage.compress_archive(enriched)
         cluster_storage.upload_and_rotate()
```

### Comparing `kubemarine-0.28.1/kubemarine/core/connections.py` & `kubemarine-0.29.0/kubemarine/core/connections.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,21 @@
 
 class ConnectionPool:
     def __init__(self, nodes: Dict[str, dict], gateway_nodes: Dict[str, dict], hosts: List[str]):
         self._nodes = nodes
         self._gateway_nodes = gateway_nodes
         self._connections: Connections = {ip: self._create_connection(ip) for ip in hosts}
 
+    def get_node(self, ip: str) -> dict:
+        node = self._nodes.get(ip)
+        if node is None:
+            raise Exception("Failed to find suitable node to connect to by address %s" % ip)
+
+        return node
+
     def get_connection(self, ip: str) -> fabric.connection.Connection:
         conn = self._connections.get(ip)
         if conn is None:
             raise Exception(f'Connection for {ip} is not registered')
 
         return conn
 
@@ -59,31 +66,28 @@
             connect_timeout=conn_details.get('connection_timeout',
                                              static.GLOBALS['connection']['defaults']['timeout']),
             connect_kwargs=creds,
             inline_ssh_env=inline_ssh_env
         )
 
     def _create_connection(self, ip: str) -> fabric.connection.Connection:
-        node = self._nodes.get(ip)
-        if node is None:
-            raise Exception("Failed to find suitable node to connect to by address %s" % ip)
+        node = self.get_node(ip)
 
         if node.get('keyfile') is None and node.get('password') is None:
             raise Exception('There is neither keyfile nor password specified in configfile for node \'%s\'' % node['name'])
 
         gateway = None
         if 'gateway' in node:
             gateway = self._get_gateway_node_connection(node['gateway'])
 
         return self._create_connection_from_details(ip, node, gateway=gateway)
 
     def _get_gateway_node_connection(self, name: str) -> fabric.connection.Connection:
         # Create new connection instance each time even if it is the same gateway node.
         # This is necessary to not share the same gateway connection instance in multiple threads
-        gateway_conn = None
 
         gateway = self._gateway_nodes.get(name)
         if gateway is None:
             raise Exception('Requested gateway \'%s\' is not found in configfile' % name)
 
         if gateway.get('address') is None:
             raise Exception('There is no address specified in configfile for gateway \'%s\'' % name)
```

### Comparing `kubemarine-0.28.1/kubemarine/core/defaults.py` & `kubemarine-0.29.0/kubemarine/core/defaults.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,21 +20,42 @@
 from kubemarine.core.errors import KME
 from kubemarine import jinja, keepalived, haproxy, controlplane, kubernetes, thirdparties
 from kubemarine.core import utils, static, log, os
 from kubemarine.core.yaml_merger import default_merger
 from kubemarine.cri.containerd import contains_old_format_properties
 
 
+supported_connection_defaults = {
+    'node_defaults': 'nodes',
+}
+
 supported_defaults = {
     'rbac': {
         'account_defaults': 'accounts'
     },
-    'node_defaults': 'nodes',
 }
 
+connection_sections = [
+    'nodes', 'node_defaults', 'gateway_nodes',
+    'procedure_history',  # Required to preserve inventory
+    'values', 'cluster_name'  # May be referred to in jinja expressions
+]
+
+ssh_access_default_properties = [
+    'keyfile', 'password', 'username', 'connection_port', 'connection_timeout', 'gateway',
+    'boot'  # Participates in workarounds and reboot. This dependency can potentially be avoided
+]
+
+ssh_access_node_properties = ssh_access_default_properties + [
+    'address', 'internal_address', 'connect_to',
+    'name',  # In context of connections, the name is used only in logging. This dependency can potentially be avoided.
+    'roles'  # Required to distinguish control planes to preserve inventory.
+]
+
+
 invalid_node_name_regex = re.compile("[^a-z-.\\d]", re.M)
 escaped_expression_regex = re.compile('({%[\\s*|]raw[\\s*|]%}.*?{%[\\s*|]endraw[\\s*|]%})', re.M)
 jinja_query_regex = re.compile("{{ .* }}", re.M)
 
 
 @enrichment(EnrichmentStage.LIGHT, procedures=['add_node'])
 def add_node_enrich_roles(cluster: KubernetesCluster) -> None:
@@ -88,14 +109,19 @@
         roles = node['roles']
         for role in ('add_node', 'remove_node'):
             if role in roles:
                 roles.remove(role)
 
 
 @enrichment(EnrichmentStage.ALL)
+def apply_connection_defaults(cluster: KubernetesCluster) -> None:
+    recursive_apply_defaults(supported_connection_defaults, cluster.inventory)
+
+
+@enrichment(EnrichmentStage.FULL)
 def apply_defaults(cluster: KubernetesCluster) -> None:
     recursive_apply_defaults(supported_defaults, cluster.inventory)
 
 
 @enrichment(EnrichmentStage.ALL)
 def calculate_connect_to(cluster: KubernetesCluster) -> None:
     for node in cluster.inventory["nodes"]:
@@ -125,16 +151,16 @@
 
             address = node['connect_to']
             ips['all'].append(address)
             for role in node['roles']:
                 if role not in ('remove_node', 'add_node'):
                     ips.setdefault(role, []).append(address)
 
-        for role in ips.keys():
-            nodes[role] = cluster.make_group(ips[role])
+        for role, hosts in ips.items():
+            nodes[role] = cluster.make_group(hosts)
 
 
 @enrichment(EnrichmentStage.FULL)
 def apply_registry(cluster: KubernetesCluster) -> None:
     inventory = cluster.inventory
 
     if not inventory.get('registry'):
@@ -232,15 +258,15 @@
     #  Probably we could make endpoints optional in this case.
     containerd_endpoints = inventory['registry']['endpoints']
     thirdparties_address = inventory['registry'].get('thirdparties')
 
     return registry_mirror_address, containerd_endpoints, thirdparties_address
 
 
-@enrichment(EnrichmentStage.ALL)
+@enrichment(EnrichmentStage.FULL)
 def append_controlplain(cluster: KubernetesCluster) -> None:
     _append_controlplain(cluster.inventory, cluster.log)
 
 
 def _append_controlplain(inventory: dict, logger: log.EnhancedLogger) -> None:
 
     if inventory.get('control_plain', {}).get('internal') and inventory.get('control_plain', {}).get('external'):
@@ -276,15 +302,16 @@
                     internal_address = item['ip']
                     internal_address_source = 'vrrp_ip[%s]' % i
                 if item.get('floating_ip') and (external_address is None or item.get('control_endpoint', False)):
                     external_address = item['floating_ip']
                     external_address_source = 'vrrp_ip[%s]' % i
 
     if internal_address is not None and external_address is None:
-        logger.warning('VRRP_IPs has an internal address, but do not have an external one. Your configuration may be incorrect. Trying to handle this problem automatically...')
+        logger.warning('VRRP_IPs has an internal address, but do not have an external one. '
+                       'Your configuration may be incorrect. Trying to handle this problem automatically...')
 
     if internal_address is None or external_address is None:
         # 'master' role is not deleted due to unit tests are not refactored
         for role in ['balancer', 'control-plane', 'master']:
             # nodes are not compiled to groups yet
             for node in inventory['nodes']:
                 if role in node['roles']:
@@ -295,31 +322,33 @@
                         external_address = node['address']
                         external_address_source = f"{role} \"{node['name']}\""
 
     if external_address is None:
         logger.warning('Failed to detect external control plain. Something may work incorrect!')
         external_address = internal_address
 
-    logger.debug('Control plains:\n   Internal: %s (%s)\n   External: %s (%s)' % (internal_address, internal_address_source, external_address, external_address_source))
+    logger.debug('Control plains:\n   Internal: %s (%s)\n   External: %s (%s)'
+                 % (internal_address, internal_address_source, external_address, external_address_source))
 
     # apply controlplain ips
     if not inventory.get('control_plain'):
         inventory['control_plain'] = {}
 
     if not inventory['control_plain'].get('internal'):
         inventory['control_plain']['internal'] = internal_address
 
     if not inventory['control_plain'].get('external'):
         inventory['control_plain']['external'] = external_address
 
 
 def recursive_apply_defaults(defaults: dict, section: dict) -> None:
     for key, value in defaults.items():
-        if isinstance(value, dict) and section.get(key) is not None and section[key]:
-            recursive_apply_defaults(value, section[key])
+        if isinstance(value, dict):
+            if section.get(key) is not None and section[key]:
+                recursive_apply_defaults(value, section[key])
         # check if target section exists and not empty
         elif section.get(value) is not None:
             for i, custom_value in enumerate(section[value]):
                 # copy defaults as new dict, to avoid problems with memory links
                 default_value = utils.deepcopy_yaml(section[key])
 
                 # update defaults with custom-defined node configs
@@ -329,17 +358,17 @@
                 # replace old node config with merged one
                 section[value][i] = default_value
 
 
 @enrichment(EnrichmentStage.ALL)
 def calculate_node_names(cluster: KubernetesCluster) -> None:
     roles_iterators: Dict[str, int] = {}
-    for i, node in enumerate(cluster.inventory['nodes']):
-        # 'master' role is not deleted because calculate_node_names() can be run over initial inventory,
-        # that still supports the old role.
+    for node in cluster.inventory['nodes']:
+        # 'master' role is not deleted because calculate_node_names() can be run over old inventory,
+        # that may still have the old role (LIGHT enrichment).
         for role_name in ['control-plane', 'master', 'worker', 'balancer']:
             if role_name in node['roles']:
                 # The idea is this:
                 # If the name is already specified, we must skip this node,
                 # however, we must consider that we already have a node of this type
                 # and increase this type iterator
                 # As a result, we get such an algorithm. For example, with the following inventory:
@@ -393,28 +422,72 @@
         node_name = gateway_node['name']
         if node_name in known_gateway_node_names:
             raise Exception(f"Gateway node name {node_name} is duplicated in configfile")
 
         known_gateway_node_names.append(node_name)
 
 
-@enrichment(EnrichmentStage.ALL)
+def restrict_connection_sections(inventory: dict) -> dict:
+    """
+    Returns shallow copy of the inventory with only those sections
+    that participate in the enrichment of connections.
+    """
+    inventory = utils.subdict_yaml(inventory, connection_sections)
+    node_defaults = inventory.get('node_defaults', {})
+    if node_defaults:
+        inventory['node_defaults'] = utils.subdict_yaml(node_defaults, ssh_access_default_properties)
+
+    nodes = inventory.get('nodes', [])
+    if nodes:
+        inventory['nodes'] = nodes = list(nodes)
+        for i, node in enumerate(nodes):
+            nodes[i] = utils.subdict_yaml(node, ssh_access_node_properties)
+
+    return inventory
+
+
+@enrichment(EnrichmentStage.LIGHT)
+def restrict_connections(cluster: KubernetesCluster) -> dict:
+    return restrict_connection_sections(cluster.inventory)
+
+
+@enrichment(EnrichmentStage.LIGHT)
+def merge_connection_defaults(cluster: KubernetesCluster) -> dict:
+    connection_defaults = restrict_connection_sections(static.DEFAULTS)
+    return _merge_inventory(cluster, connection_defaults)
+
+
+@enrichment(EnrichmentStage.FULL)
 def merge_defaults(cluster: KubernetesCluster) -> dict:
-    base_inventory = utils.deepcopy_yaml(static.DEFAULTS)
+    return _merge_inventory(cluster, static.DEFAULTS)
+
+
+def _merge_inventory(cluster: KubernetesCluster, base: dict) -> dict:
+    base_inventory = utils.deepcopy_yaml(base)
     inventory: dict = default_merger.merge(base_inventory, cluster.inventory)
     return inventory
 
 
-@enrichment(EnrichmentStage.ALL)
+@enrichment(EnrichmentStage.LIGHT)
+def compile_connections(cluster: KubernetesCluster) -> None:
+    return _compile_inventory(cluster, inject_globals=False)
+
+
+@enrichment(EnrichmentStage.FULL)
 def compile_inventory(cluster: KubernetesCluster) -> None:
+    return _compile_inventory(cluster, inject_globals=True)
+
+
+def _compile_inventory(cluster: KubernetesCluster, *, inject_globals: bool) -> None:
     inventory = cluster.inventory
     # convert references in yaml to normal values
     iterations = 100
     root = utils.deepcopy_yaml(inventory)
-    root['globals'] = static.GLOBALS
+    if inject_globals:
+        root['globals'] = static.GLOBALS
     root['env'] = os.Environ()
 
     while iterations > 0:
 
         cluster.log.verbose('Inventory is not rendered yet...')
         inventory = compile_object(cluster.log, inventory, root)
 
@@ -571,15 +644,15 @@
             value = value.strip()
         if strip and value == '':
             del struct[section]  # type: ignore[arg-type]
         else:
             try:
                 struct[section] = func(value)  # type: ignore[index]
             except ValueError as e:
-                raise ValueError(f"{str(e)} in section [{']['.join(repr(p) for p in path)}]")
+                raise ValueError(f"{str(e)} in section [{']['.join(repr(p) for p in path)}]") from None
 
     path.pop()
 
 
 def _set_overridden_blank_primitive_values(raw_struct: Union[dict, list], struct: Union[dict, list],
                                            path: List[Union[str, int]],
                                            search_path: List[str]) -> None:
```

### Comparing `kubemarine-0.28.1/kubemarine/core/environment.py` & `kubemarine-0.29.0/kubemarine/core/environment.py`

 * *Files 23% similar despite different names*

```diff
@@ -18,19 +18,14 @@
 from kubemarine.core import log
 from kubemarine.core.connections import ConnectionPool
 
 
 class Environment(ABC):
     @property
     @abstractmethod
-    def inventory(self) -> dict:
-        pass
-
-    @property
-    @abstractmethod
     def connection_pool(self) -> ConnectionPool:
         pass
 
     @property
     @abstractmethod
     def log(self) -> log.EnhancedLogger:
         pass
```

### Comparing `kubemarine-0.28.1/kubemarine/core/errors.py` & `kubemarine-0.29.0/kubemarine/core/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from textwrap import dedent
 from typing import Type, List
 
 from kubemarine.core import log as klog
 
 
 def get_kme_dictionary() -> dict:
-    from kubemarine.core.group import GroupException
+    from kubemarine.core.group import GroupException  # pylint: disable=cyclic-import
     return {
         "KME0000": {
             "name": "Test exception"
         },
         "KME0002": {
             "instance": GroupException,
             "name": "Remote group exception\n{reason}"
@@ -86,15 +86,15 @@
                     "but not present in procedure inventory{next_version_spec}. "
                     "Please, specify required 'sandbox_image' explicitly in procedure inventory."
         }
     }
 
 
 class _BaseKME(RuntimeError, ABC):
-    def __init__(self, code: str, **kwargs: object):
+    def __init__(self, code: str):
         self.code = code
         if self.code not in get_kme_dictionary():
             raise ValueError('An error was raised with an unknown error code')
         self.kme: dict = get_kme_dictionary()[self.code]
         self.message = self._format()
         super().__init__(self.message)
```

### Comparing `kubemarine-0.28.1/kubemarine/core/executor.py` & `kubemarine-0.29.0/kubemarine/core/executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,23 +14,22 @@
 import collections
 import concurrent
 import io
 import random
 import re
 import time
 from abc import ABC, abstractmethod
+from concurrent.futures import ThreadPoolExecutor
 from datetime import datetime
 from types import TracebackType
 from typing import Tuple, List, Dict, Callable, Any, Optional, Union, OrderedDict, TypeVar, Type, Mapping, Iterable
 
 import fabric  # type: ignore[import-untyped]
 import fabric.transfer  # type: ignore[import-untyped]
 
-from concurrent.futures.thread import ThreadPoolExecutor
-
 import invoke
 
 from kubemarine.core import log, static
 from kubemarine.core.connections import ConnectionPool
 from kubemarine.core.environment import Environment
 
 EXIT_CODE_PATTERN = re.compile(r'^\n(\d+)\n')
@@ -200,15 +199,14 @@
 
     def __init__(self, cluster: Environment, connection_pool: ConnectionPool = None) -> None:
         self.logger = cluster.log
         if connection_pool is not None:
             self.connection_pool = connection_pool
         else:
             self.connection_pool = cluster.connection_pool
-        self.inventory = cluster.inventory
         self._connections_queue: Dict[str, List[_PayloadItem]] = {}
         self._last_token = -1
         self._last_results: Dict[str, TokenizedResult] = {}
         self._command_separator = ''.join(random.choice('=-_') for _ in range(32))
         self._supported_args = {'hide', 'warn', 'timeout', 'env', 'out_stream', 'err_stream'}
         self._closed = False
 
@@ -253,15 +251,15 @@
         reparsed_results: Dict[str, TokenizedResult] = {}
         for host, raw_result in raw_results.items():
             payloads = batch[host]
             conn_results: TokenizedResult = collections.OrderedDict()
             reparsed_results[host] = conn_results
 
             runner_exception = None
-            if isinstance(raw_result, invoke.UnexpectedExit) or isinstance(raw_result, invoke.CommandTimedOut):
+            if isinstance(raw_result, (invoke.UnexpectedExit, invoke.CommandTimedOut)):
                 runner_exception = raw_result
                 raw_result = raw_result.result
 
             if not isinstance(raw_result, fabric.runners.Result):
                 token = payloads[0][2]
                 conn_results[token] = raw_result
                 continue
@@ -387,17 +385,17 @@
         while True:
             batch: Dict[str, List[_PayloadItem]] = {}
             for host, actions in callables.items():
                 if len(actions) > i:
                     batch[host] = actions[i]
             if not batch:
                 break
-            else:
-                i += 1
-                batches.append(batch)
+
+            i += 1
+            batches.append(batch)
 
         return batches
 
     def _next_token(self) -> int:
         self._last_token += 1
         return self._last_token
 
@@ -529,21 +527,24 @@
                 result_map[host] = call()
             except Exception as e:
                 results[host] = e
 
         for host, payloads in batch.items():
             cxn = self.connection_pool.get_connection(host)
             do_type, args, kwargs = self._prepare_merged_action(host, payloads)
+            # pylint: disable-next=cell-var-from-loop
             safe_exec(futures, host, lambda: tpe.submit(getattr(cxn, do_type), *args, **kwargs))
 
         for host, future in futures.items():
             # We try to shut down ThreadPoolExecutor gracefully with joining of all the threads.
             # This makes usage of future timeout useless, as the operation is not stopped.
             # Instead, we always pass timeout for run/sudo and so have CommandTimedOut.
             # For put/get fabric & paramiko do not offer timeout, so transfer cannot be stopped currently.
+
+            # pylint: disable-next=cell-var-from-loop
             safe_exec(results, host, lambda: future.result(timeout=None))
 
         self._flush_logger_writers(batch)
 
         return self._reparse_results(results, batch)
 
     def _get_remained_batch(self, batch: Dict[str, List[_PayloadItem]],
@@ -603,22 +604,19 @@
 
     def wait_for_boot(self, left_nodes: List[str], timeout: int = None,
                       initial_boot_history: Mapping[str, RunnersResult] = None) -> HostToResult:
         with ThreadPoolExecutor(max_workers=len(left_nodes)) as TPE:
             return self._wait_for_boot_with_executor(left_nodes, TPE, timeout, initial_boot_history)
 
     def _wait_for_boot_with_executor(self, left_nodes: List[str], tpe: ThreadPoolExecutor,
-                                     timeout: int = None,
+                                     overridden_timeout: int = None,
                                      initial_boot_history: Mapping[str, RunnersResult] = None) -> HostToResult:
 
-        boot_config = self._get_boot_config()
-        if timeout is None:
-            timeout = boot_config['timeout']
-
-        delay_period = boot_config['defaults']['delay_period']
+        timeout = self._resolve_boot_timeout(left_nodes, overridden_timeout)
+        delay_period = static.GLOBALS['nodes']['boot']['defaults']['delay_period']
 
         if initial_boot_history is None:
             initial_boot_history = {}
 
         results: HostToResult = {}
         time_start = datetime.now()
 
@@ -637,22 +635,24 @@
                           if (isinstance(result, Exception)
                               # Something is wrong with sudo access. Node is active.
                               and not self.is_require_nopasswd_exception(result))
                           or (not isinstance(result, Exception)
                               and result == initial_boot_history.get(host))]
 
             waited = (datetime.now() - time_start).total_seconds()
+            if left_nodes:
+                timeout = self._resolve_boot_timeout(left_nodes, overridden_timeout)
 
             if not left_nodes or waited >= timeout:
                 break
 
             for host, exc in results.items():
                 if isinstance(exc, Exception) and not self._is_allowed_connection_exception(str(exc)):
                     self.logger.verbose("Unexpected exception at %s, node is considered as not booted: %s"
-                                             % (host, str(exc)))
+                                        % (host, str(exc)))
 
             self.logger.verbose("Nodes %s are not ready yet, remaining time to wait %i"
                                 % (left_nodes, timeout - waited))
 
             attempt_time = (datetime.now() - attempt_time_start).total_seconds()
             if attempt_time < delay_period:
                 time.sleep(delay_period - attempt_time)
@@ -660,18 +660,23 @@
         if left_nodes:
             self.logger.verbose("Failed to wait for boot of nodes %s" % left_nodes)
         else:
             self.logger.verbose("All nodes are online now")
 
         return results
 
-    def _get_boot_config(self) -> dict:
-        boot_config = dict(self.inventory['globals']['nodes']['boot'])
-        boot_config.update(static.GLOBALS['nodes']['boot'])
-        return boot_config
+    def _resolve_boot_timeout(self, hosts: List[str], overridden_timeout: Optional[int]) -> int:
+        if overridden_timeout is not None:
+            return overridden_timeout
+
+        return max(self._get_node_boot_timeout(host) for host in hosts)
+
+    def _get_node_boot_timeout(self, host: str) -> int:
+        timeout: int = self.connection_pool.get_node(host)['boot']['timeout']
+        return timeout
 
     def _do_nopasswd(self, left_nodes: List[str], tpe: ThreadPoolExecutor, command: str) -> HostToResult:
         prompt = '[sudo] password: '
 
         class NoPasswdResponder(invoke.Responder):
             def __init__(self) -> None:
                 super().__init__(re.escape(prompt), "")
```

### Comparing `kubemarine-0.28.1/kubemarine/core/flow.py` & `kubemarine-0.29.0/kubemarine/core/flow.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 import argparse
 import os
 import shlex
 import sys
 import time
 from abc import abstractmethod, ABC
 from copy import deepcopy
-from types import FunctionType
-from typing import Optional, List, Union, Sequence, Tuple, cast, Callable, Dict, Any
+from typing import Optional, List, Union, Sequence, Tuple, Dict, Any
 
 from kubemarine.core import utils, cluster as c, action, resources as res, errors, summary, log, defaults
 
 ERROR_UNRECOGNIZED_CUMULATIVE_POINT_EXCLUDE = "Unrecognized cumulative point to exclude: {point}"
 ERROR_UNRECOGNIZED_TASKS_FILTER = "Unrecognized tasks filter: {tasks}"
 
 TASK_DESCRIPTION_TEMPLATE = """
@@ -110,77 +109,90 @@
                 with utils.open_external(resources.inventory_filepath, "r") as stream:
                     utils.dump_file(context, stream, "cluster_initial.yaml")
 
             if resources.procedure_inventory_filepath:
                 with utils.open_external(resources.procedure_inventory_filepath, "r") as stream:
                     utils.dump_file(context, stream, "procedure.yaml")
 
-        if cluster is None:
-            # We currently do not support inventory preservation for actions that only change the inventory
-            successfully_performed = []
+        # Initialize connections early, in particular for inventory preservation.
+        resources.cluster(c.EnrichmentStage.LIGHT)
 
         try:
             logger.info(f"Running action '{act.identifier}'")
             act.run(resources)
             resources.collect_action_result()
             successfully_performed.append(act.identifier)
         except Exception:
             if successfully_performed:
-                _post_process_actions_group(resources, successfully_performed, failed=True)
+                _post_process_actions_group(resources, cluster, successfully_performed, failed=True)
 
             raise
 
         cluster = resources.cluster_if_initialized()
 
         if act.recreate_inventory:
             if resources.inventory_filepath:
                 with utils.open_external(resources.inventory_filepath, "r") as stream:
                     # write original file data to backup file with timestamp
                     timestamp = utils.get_current_timestamp_formatted()
                     inventory_file_basename = os.path.basename(resources.inventory_filepath)
                     utils.dump_file(context, stream, "%s_%s" % (inventory_file_basename, str(timestamp)))
 
             resources.recreate_inventory()
-            _post_process_actions_group(resources, successfully_performed)
+            _post_process_actions_group(resources, cluster, successfully_performed)
             successfully_performed = []
+            cluster = None
 
     if successfully_performed:
-        _post_process_actions_group(resources, successfully_performed)
+        _post_process_actions_group(resources, cluster, successfully_performed)
 
 
-def _post_process_actions_group(resources: res.DynamicResources, successfully_performed: List[str],
+def _post_process_actions_group(resources: res.DynamicResources, cluster: Optional[c.KubernetesCluster],
+                                successfully_performed: List[str],
                                 *,
                                 failed: bool = False) -> None:
-    if resources.cluster_if_initialized() is None:
-        return
+    previous_successful_cluster = cluster is not None
+    try:
+        if previous_successful_cluster:
+            _dump_inventory(resources, failed)
+    finally:
+        _preserve_inventory(resources, successfully_performed, failed=failed, enriched=previous_successful_cluster)
 
+
+def _dump_inventory(resources: res.DynamicResources, failed: bool) -> None:
     context = resources.context
 
     # If cluster is initialized, it is fully enriched at least to DEFAULT state.
     # Use this state to dump all effective inventories.
     # This is acceptable due to the following assumptions for the last action:
     # * If successful, changes in the inventory should be moved to this state in DynamicResources.recreate_inventory().
     # * If failed, switch to this state effectively restores the cluster to the state after previous action succeeded.
     cluster = resources.cluster(c.EnrichmentStage.DEFAULT)
-    try:
-        if failed:
-            # Preserve effective inventory for the last succeeded action.
-            # For debug aims, cluster_procedure.yaml can still be used.
-            defaults.dump_inventory(cluster, context, 'cluster.yaml')
 
-        resources.dump_finalized_inventory(cluster)
-    finally:
-        context['successfully_performed'] = successfully_performed
-        context['status'] = 'failed' if failed else 'successful'
+    if failed:
+        # Preserve effective inventory for the last succeeded action.
+        # For debug aims, cluster_procedure.yaml can still be used.
+        defaults.dump_inventory(cluster, context, 'cluster.yaml')
+
+    resources.dump_finalized_inventory(cluster)
+
+
+def _preserve_inventory(resources: res.DynamicResources, successfully_performed: List[str],
+                        *,
+                        failed: bool, enriched: bool) -> None:
+    context = resources.context
+
+    context['successfully_performed'] = successfully_performed
+    context['status'] = 'failed' if failed else 'successful'
 
-        if (resources.context['preserve_inventory']
-                and not resources.context['execution_arguments'].get('without_act', False)):
-            # If the main cluster is initialized, light cluster is initialized for sure
-            cluster = resources.cluster(c.EnrichmentStage.LIGHT)
-            cluster.preserve_inventory(context)
+    if (resources.context['preserve_inventory']
+            and not resources.context['execution_arguments'].get('without_act', False)):
+        # Light cluster is always pre-initialized before running of any action.
+        cluster = resources.cluster(c.EnrichmentStage.LIGHT)
+        cluster.preserve_inventory(context, enriched=enriched)
 
 
 class TasksAction(action.Action):
     def __init__(self, identifier: str, tasks: dict,
                  *,
                  cumulative_points: dict = None,
                  tasks_filter: List[str] = None,
@@ -215,27 +227,28 @@
             return
 
         init_tasks_flow(cluster)
         run_tasks_recursive(self.tasks, final_list, cluster, self.cumulative_points, [])
         proceed_cumulative_point(cluster, self.cumulative_points, END_OF_TASKS,
                                  force=args.get('force_cumulative_points', False))
 
-    def cluster(self, resources: res.DynamicResources) -> c.KubernetesCluster:
-        return resources.cluster()
+    def cluster(self, _res: res.DynamicResources) -> c.KubernetesCluster:
+        return _res.cluster()
 
 
 def run_tasks(resources: res.DynamicResources, tasks: dict, cumulative_points: dict = None) -> None:
     return TasksAction("", tasks, cumulative_points=cumulative_points).run(resources)
 
 
 def create_empty_context(args: dict, procedure: str) -> dict:
     return {
         "execution_arguments": deepcopy(args),
         'initial_procedure': procedure,
         'preserve_inventory': True,
+        'make_finalized_inventory': True,
         'load_inventory_silent': False,
         'runtime_vars': {},
         'result': ['summary_report'],
     }
 
 
 def get_task_list(tasks: dict, _task_path: str = '', leafs_only: bool = True) -> List[str]:
@@ -465,38 +478,14 @@
 
     if args.workdir != '':
         os.chdir(args.workdir)
 
     return args
 
 
-def schedule_cumulative_point(cluster: c.KubernetesCluster, point_method: Callable) -> None:
-    _check_within_flow(cluster)
-
-    func = cast(FunctionType, point_method)
-    point_fullname = func.__module__ + '.' + func.__qualname__
-
-    if cluster.context['execution_arguments'].get('disable_cumulative_points', False):
-        cluster.log.verbose('Method %s not scheduled - cumulative points disabled' % point_fullname)
-        return
-
-    if point_fullname in cluster.context['execution_arguments']['exclude_cumulative_points_methods']:
-        cluster.log.verbose('Method %s not scheduled - it set to be excluded' % point_fullname)
-        return
-
-    scheduled_points = cluster.context.get('scheduled_cumulative_points', [])
-
-    if point_method not in scheduled_points:
-        scheduled_points.append(point_method)
-        cluster.context['scheduled_cumulative_points'] = scheduled_points
-        cluster.log.verbose('Method %s scheduled' % point_fullname)
-    else:
-        cluster.log.verbose('Method %s already scheduled' % point_fullname)
-
-
 def proceed_cumulative_point(cluster: c.KubernetesCluster, points_list: dict,
                              point_task_name: Union[str, object], force: bool = False) -> Dict[str, Any]:
     _check_within_flow(cluster)
 
     if cluster.context['execution_arguments'].get('disable_cumulative_points', False):
         return {}
 
@@ -525,20 +514,15 @@
 
 def init_tasks_flow(cluster: c.KubernetesCluster) -> None:
     if 'proceeded_tasks' not in cluster.context:
         cluster.context['proceeded_tasks'] = []
 
 
 def add_task_to_proceeded_list(cluster: c.KubernetesCluster, task_path: str) -> None:
-    if not is_task_completed(cluster, task_path):
+    if not cluster.is_task_completed(task_path):
         cluster.context['proceeded_tasks'].append(task_path)
         utils.dump_file(cluster, "\n".join(cluster.context['proceeded_tasks'])+"\n", 'finished_tasks')
 
 
-def is_task_completed(cluster: c.KubernetesCluster, task_path: str) -> bool:
-    _check_within_flow(cluster)
-    return task_path in cluster.context['proceeded_tasks']
-
-
 def _check_within_flow(cluster: c.KubernetesCluster, check: bool = True) -> None:
     if check != ('proceeded_tasks' in cluster.context):
         raise NotImplementedError(f"The method is called {'not ' if check else ''}within tasks flow execution")
```

### Comparing `kubemarine-0.28.1/kubemarine/core/group.py` & `kubemarine-0.29.0/kubemarine/core/group.py`

 * *Files 1% similar despite different names*

```diff
@@ -269,15 +269,15 @@
 RunResult = Union[RunnersGroupResult, Token]
 GROUP_RUN_TYPE = TypeVar('GROUP_RUN_TYPE', bound=RunResult, covariant=True)
 GROUP_SELF = TypeVar('GROUP_SELF', bound='AbstractGroup[Union[RunnersGroupResult, Token]]')
 
 
 class AbstractGroup(Generic[GROUP_RUN_TYPE], ABC):
     def __init__(self, ips: Iterable[Union[str, GROUP_SELF]], cluster: object):
-        from kubemarine.core.cluster import KubernetesCluster
+        from kubemarine.core.cluster import KubernetesCluster  # pylint: disable=cyclic-import
 
         self.cluster = cast(KubernetesCluster, cluster)
         self.nodes: Set[str] = set()
         for ip in ips:
             if isinstance(ip, self.__class__):
                 for host in ip.nodes:
                     self.nodes.add(host)
@@ -368,14 +368,15 @@
             if not hosts_to_upload:
                 self.cluster.log.verbose('Local and remote hashes are equal on all nodes, no transmission required')
                 return
 
             local_stream = local_file
             group_to_upload = self._make_group(hosts_to_upload)
 
+        # pylint: disable-next=protected-access
         group_to_upload._put_with_mv(local_stream, remote_file,
                                      backup=backup, sudo=sudo, mkdir=mkdir, immutable=immutable)
 
     def _put_with_mv(self, local_stream: Union[io.BytesIO, str], remote_file: str,
                      backup: bool, sudo: bool, mkdir: bool, immutable: bool) -> None:
 
         if sudo:
@@ -490,37 +491,40 @@
         # Added nodes will be at the end thus reproducing the procedure enrichment.
         for node in itertools.chain(self.cluster.previous_inventory['nodes'], self.cluster.inventory['nodes']):
             host = node['connect_to']
             # is iterable node from inventory is part of current NodeGroup?
             if host not in self.nodes:
                 continue
 
+            if apply_filter is None:
+                result[host] = node
+                continue
+
             # apply filters
             suitable = True
-            if apply_filter is not None:
-                if callable(apply_filter):
-                    if not apply_filter(node):
+            if callable(apply_filter):
+                if not apply_filter(node):
+                    suitable = False
+            else:
+                # here intentionally there is no way to filter by values in lists field,
+                # for this you need to use custom functions.
+                # Current solution implemented in this way because the filtering strategy is
+                # unclear - do I need to include when everything matches or is partial matching enough?
+                for key, value in apply_filter.items():
+                    if node.get(key) is None:
                         suitable = False
-                else:
-                    # here intentionally there is no way to filter by values in lists field,
-                    # for this you need to use custom functions.
-                    # Current solution implemented in this way because the filtering strategy is
-                    # unclear - do I need to include when everything matches or is partial matching enough?
-                    for key, value in apply_filter.items():
-                        if node.get(key) is None:
-                            suitable = False
-                            break
-                        if isinstance(value, list):
-                            if node[key] not in value:
-                                suitable = False
-                                break
-                        # elif should definitely be here, not if
-                        elif node[key] != value:
+                        break
+                    if isinstance(value, list):
+                        if node[key] not in value:
                             suitable = False
                             break
+                    # elif should definitely be here, not if
+                    elif node[key] != value:
+                        suitable = False
+                        break
 
             # if not filtered
             if suitable:
                 result[host] = node
 
         return list(result.values())
 
@@ -749,15 +753,15 @@
                 defer.flush()
             except RemoteGroupException as e:
                 results = e.results[self.get_host()]
                 for result in results:
                     if isinstance(result, UnexpectedExit):
                         logger.debug(result.result.stderr)
                         break
-                    elif isinstance(result, Exception):
+                    if isinstance(result, Exception):
                         raise
 
                     del remained_commands[0]
 
                 return False
 
             return True
@@ -816,15 +820,15 @@
         return AbstractGroup.exclude_group(self, group)
 
     def intersection_group(self, group: DeferredGroup) -> DeferredGroup:
         self._check_same_bound_executor(group)
         return AbstractGroup.intersection_group(self, group)
 
     def _check_same_bound_executor(self, group: DeferredGroup) -> None:
-        if self._executor is not group._executor:
+        if self._executor is not group._executor:  # pylint: disable=protected-access
             raise ValueError("Trying to apply set operation on deferred groups bound to different executors")
 
 
 class RemoteExecutor(RawExecutor):
     def __init__(self, group: NodeGroup, connection_pool: ConnectionPool = None) -> None:
         super().__init__(group.cluster, connection_pool)
         self.group: DeferredGroup = group._make_defer(self)
@@ -835,15 +839,15 @@
         Flushes the connections' queue.
         Throws GroupException in case of any failure.
 
         :return: grouped tokenized results per connection.
         """
         super().flush()
 
-        for host, results in self._last_results.items():
+        for results in self._last_results.values():
             if any(isinstance(result, Exception) for _, result in results.items()):
                 raise RemoteGroupException(self.cluster, self._last_results)
 
 
 class GroupException(Exception):
     def __init__(self, cluster: object, results: Dict[str, List[GenericResult]]):
         self.cluster = cluster
```

### Comparing `kubemarine-0.28.1/kubemarine/core/log.py` & `kubemarine-0.29.0/kubemarine/core/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,19 +12,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
 import os
 import sys
 from abc import ABC, abstractmethod
+from typing import Any, List, Optional, cast, Dict, Union
 
 from pygelf import gelf, GelfTcpHandler, GelfUdpHandler, GelfTlsHandler, GelfHttpHandler  # type: ignore[import-untyped]
 
-from typing import Any, List, Optional, cast, Dict, Union
-
 VERBOSE = 5
 gelf.LEVELS.update({VERBOSE: 8})
 
 DEFAULT_FORMAT = '%(asctime)s %(name)s %(levelname)s %(message)s'
 
 BLACK, RED, GREEN, YELLOW, BLUE, MAGENTA, CYAN, WHITE = range(8)
 
@@ -193,22 +192,22 @@
 
     def __init__(self,
                  target: str,
                  level: str,
                  colorize: bool = False,
                  correct_newlines: bool = False,
                  filemode: str = 'a',
-                 format: str = DEFAULT_FORMAT,
+                 format_: str = DEFAULT_FORMAT,
                  datefmt: str = None,
                  header: str = None,
                  **kwargs: Union[str, bool, int]):
 
         self._colorize = colorize
         self._correct_newlines = correct_newlines
-        self._format = format
+        self._format = format_
         self._datefmt = datefmt
         self._header = header
 
         self._formatter = LogFormatter(self._format, self._datefmt,
                                        colorize=self._colorize,
                                        correct_newlines=self._correct_newlines)
 
@@ -252,23 +251,25 @@
                 raise Exception(f'Unknown Graylog type "{kwargs["type"]}" for "{kwargs["host"]}:{kwargs["port"]}"')
 
             self.handler.setFormatter(self._formatter)
         else:
             self._target = target
             # Output produced by remote commands might contain characters which cannot be encoded on Windows deployer.
             # Specify explicitly utf-8 encoding which is native to the remote machines.
-            self.handler = FileHandlerWithHeader(self._formatter, self._target, mode=filemode, header=self._header, encoding='utf-8')
+            self.handler = FileHandlerWithHeader(self._formatter, self._target,
+                                                 mode=filemode, header=self._header, encoding='utf-8')
 
         if level not in LOGGING_LEVELS_BY_NAME:
             raise Exception(f'Failed to create logger - unknown logging level: "{level}"')
         self._level = LOGGING_LEVELS_BY_NAME[level]
         self.handler.setLevel(self._level)
 
     def __str__(self) -> str:
-        return f'target: {self._target}, level: {LOGGING_NAMES_BY_LEVEL[self._level]}, colorize: {self._colorize}, datefmt: {self._datefmt}, format: {self._format}'
+        return (f'target: {self._target}, level: {LOGGING_NAMES_BY_LEVEL[self._level]}, '
+                f'colorize: {self._colorize}, datefmt: {self._datefmt}, format: {self._format}')
 
     def append_to_logger(self, logger: EnhancedLogger) -> None:
         logger.addHandler(self.handler)
 
     def has_stdout_target(self) -> bool:
         return self._target == 'stdout'
 
@@ -334,15 +335,15 @@
         raise Exception('Defined logger do not contain parameters')
     target = argument_parts[0]
     level: Optional[str] = None
     for parameter in argument_parts[1:]:
         if parameter == '':
             continue
         value: Union[str, bool, int]
-        key, value, *rest = parameter.split('=')
+        key, value, *_ = parameter.split('=')
         if key == 'level':
             level = value
         else:
             if key in ['colorize', 'correct_newlines', 'debug', 'compress', 'validate']:
                 value = value.lower() in ['true', '1']
             elif key in ['chunk_size', 'timeout', 'port']:
                 value = int(value)
@@ -358,20 +359,20 @@
     args = context['execution_arguments']
     if args['disable_dump']:
         return None
 
     return os.path.join(args['dump_location'], 'dump', 'debug.log')
 
 
-def init_log_from_context_args(globals: dict, context: dict, name: str) -> Log:
+def init_log_from_context_args(globals_: dict, context: dict, name: str) -> Log:
     """
     Create Log from raw CLI arguments in Cluster context
-    :param globals: parsed globals collection
+    :param globals_: parsed globals collection
     :param context: context holding execution arguments.
-    :param raw_inventory: parsed but not yet enriched inventory
+    :param name: desirable logger name
     :return: Initialized Log, based on all parsed logging arguments
     """
 
     handlers = []
     stdout_specified = False
 
     args = context['execution_arguments']
@@ -384,18 +385,18 @@
                 else:
                     stdout_specified = True
             handlers.append(handler)
 
     debug_filepath = get_dump_debug_filepath(context)
     if debug_filepath:
         handlers.append(LogHandler(target=debug_filepath,
-                                   **globals['logging']['default_targets']['dump']))
+                                   **globals_['logging']['default_targets']['dump']))
 
     if not stdout_specified:
-        stdout_settings = globals['logging']['default_targets']['stdout']
+        stdout_settings = globals_['logging']['default_targets']['stdout']
         handlers.append(LogHandler(target='stdout', **stdout_settings))
 
     log = Log(name, handlers)
 
     log.logger.verbose('Using the following loggers: \n\t%s' % "\n\t".join("- " + str(x) for x in handlers))
 
     return log
```

### Comparing `kubemarine-0.28.1/kubemarine/core/os.py` & `kubemarine-0.29.0/kubemarine/core/os.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/core/patch.py` & `kubemarine-0.29.0/kubemarine/core/patch.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,18 @@
 
 from kubemarine.core.action import Action
 
 
 @total_ordering
 class _Priority(enum.Enum):
     INVENTORY_ONLY = 0
-    "The patch should only change the inventory. Enrichment is prohibited."
+    """
+    The patch may change the inventory.
+    The patch can run only LIGHT enrichment, and connect to nodes for read-only aims.
+    """
 
     SOFTWARE_UPGRADE = 1
     "This is a service patch that should be instantiated only automatically by migrate_kubemarine.py"
 
     REGULAR = 2
     """
     The patch can access and make some operations on the cluster.
@@ -53,16 +56,16 @@
     @abstractmethod
     def description(self) -> str:
         pass
 
 
 class InventoryOnlyPatch(Patch, ABC):
     """
-    The patch should only change the inventory.
-    Enrichment is prohibited. Calling DynamicResources.cluster() is prohibited.
+    The patch may change the inventory.
+    Calling DynamicResources.cluster(EnrichmentStage.LIGHT) is allowed to connect to nodes for read-only aims.
 
     Patches if this type are executed first.
     """
 
     def priority(self) -> _Priority:
         return _Priority.INVENTORY_ONLY
```

### Comparing `kubemarine-0.28.1/kubemarine/core/resources.py` & `kubemarine-0.29.0/kubemarine/core/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,16 @@
 import kubemarine.plugins.calico
 import kubemarine.plugins.kubernetes_dashboard
 import kubemarine.plugins.local_path_provisioner
 import kubemarine.plugins.nginx_ingress
 import kubemarine.system
 import kubemarine.thirdparties
 
-from kubemarine.core import utils, cluster as c, log, errors, static
+from kubemarine.core import cluster as c  # pylint: disable=reimported
+from kubemarine.core import utils, log, errors, static
 from kubemarine.core.connections import ConnectionPool
 from kubemarine.core.yaml_merger import default_merger
 
 
 class DynamicResources:
     def __init__(self, context: dict) -> None:
         self.context = context
@@ -131,26 +132,25 @@
     def _load_inventory(self) -> dict:
         if not self.inventory_filepath:
             raise Exception("Path to inventory is not defined")
         logger = self._logger
         msg = "Loading inventory file '%s'" % self.inventory_filepath
         if logger is None:
             if not self.context['load_inventory_silent']:
-                print(msg)
+                print(msg)  # pylint: disable=bad-builtin
         else:
             logger.info(msg)
         try:
             with utils.open_external(self.inventory_filepath) as stream:
                 # load inventory as ruamel.yaml to save original structure
                 inventory: dict = utils.yaml_structure_preserver().load(stream)
 
             return inventory
         except ruamel.yaml.YAMLError as exc:
             utils.do_fail("Failed to load inventory file", exc, logger=logger)
-            return {}  # unreachable
 
     def recreate_inventory(self) -> None:
         """
         Recreate initial inventory file using KubernetesCluster.formatted_inventory if the cluster is initialized,
         or this `inventory()` otherwise.
         Also, reset all dependent resources.
 
@@ -280,22 +280,22 @@
             # The cluster should be already enriched at DEFAULT stage to avoid unintended impact on it.
             raise ValueError(f"Cluster is not initialized at {stage.name!r} stage yet")
 
         self._clusters.pop(c.EnrichmentStage.PROCEDURE, None)
 
     def dump_finalized_inventory(self, cluster: c.KubernetesCluster) -> None:
         finalized_filename = "cluster_finalized.yaml"
-        if not self._make_finalized_inventory(finalized_filename):
+        if not self.context['make_finalized_inventory']:
             return
 
-        finalized_inventory = cluster.make_finalized_inventory(self.finalization_functions())
+        finalized_inventory = self.make_finalized_inventory(cluster)
         self._store_finalized_inventory(finalized_inventory, finalized_filename)
 
-    def _make_finalized_inventory(self, finalized_filename: str) -> bool:
-        return utils.is_dump_allowed(self.context, finalized_filename)
+    def make_finalized_inventory(self, cluster: c.KubernetesCluster) -> dict:
+        return cluster.make_finalized_inventory(self.finalization_functions())
 
     def _store_finalized_inventory(self, finalized_inventory: dict, finalized_filename: str) -> None:
         data = yaml.dump(finalized_inventory)
         utils.dump_file(self.context, data, finalized_filename)
         utils.dump_file(self.context, data, finalized_filename, dump_location=False)
 
     def collect_action_result(self) -> None:
@@ -378,14 +378,15 @@
         ).logger
 
     def enrichment_functions(self) -> List[c.EnrichmentFunction]:
         # Information about the nodes should be collected within system.detect_nodes_context().
         # All other enrichment procedures should not connect to any node.
         return [
             # JSON validation
+            kubemarine.core.schema.verify_connections,
             kubemarine.core.schema.verify_inventory,
 
             # Early enrichment of procedure inventory for connections
             kubemarine.core.defaults.add_node_enrich_roles,
             kubemarine.core.defaults.enrich_add_nodes,
             kubemarine.core.defaults.calculate_node_names,
             kubemarine.core.defaults.remove_node_enrich_roles,
@@ -404,29 +405,32 @@
             kubemarine.thirdparties.enrich_procedure_inventory,
             kubemarine.cri.enrich_upgrade_inventory,
             kubemarine.cri.containerd.enrich_migrate_cri_inventory,
             kubemarine.plugins.nginx_ingress.cert_renew_enrichment,
             # Enrichment of procedure inventory should be finished at this step.
 
             # Convert formatted inventory to native python objects, and merge defaults.
+            kubemarine.core.defaults.restrict_connections,
             kubemarine.core.cluster.KubernetesCluster.convert_formatted_inventory,
+            kubemarine.core.defaults.merge_connection_defaults,
             kubemarine.core.defaults.merge_defaults,
 
             # Pre-compilation
             kubemarine.controlplane.controlplane_node_enrichment,
             kubemarine.core.defaults.append_controlplain,
 
             # Jinja2 compilation
+            kubemarine.core.defaults.compile_connections,
             kubemarine.core.defaults.compile_inventory,
 
             # Early conversion and validation after compilation.
             # Also, complete minimal enrichment of connections.
             kubemarine.core.defaults.calculate_connect_to,
             kubemarine.core.defaults.verify_nodes,
-            kubemarine.core.defaults.apply_defaults,
+            kubemarine.core.defaults.apply_connection_defaults,
             kubemarine.core.defaults.calculate_nodegroups,
             kubemarine.core.defaults.remove_service_roles,
             # Enrichment of inventory for LIGHT stage should be finished at this step.
 
             # Should be just after compilation, but currently not necessary for LIGHT stage.
             # Sections with primitive values may be potentially split in the future if necessary for LIGHT.
             kubemarine.core.defaults.manage_primitive_values,
@@ -442,23 +446,25 @@
             kubemarine.packages.verify_procedure_inventory,
             kubemarine.plugins.verify_upgrade_inventory,
             kubemarine.thirdparties.verify_procedure_inventory,
             kubemarine.cri.verify_upgrade_inventory,
 
             # Remained default enrichment.
             # Many functions depend on kubemarine.core.defaults.calculate_nodegroups
+            kubemarine.core.defaults.apply_defaults,
             kubemarine.packages.enrich_inventory,
             kubemarine.core.defaults.apply_registry,
             kubemarine.keepalived.enrich_inventory_apply_defaults,
             kubemarine.keepalived.enrich_inventory_calculate_nodegroup,
             # Depends on kubemarine.keepalived.enrich_inventory_apply_defaults
             kubemarine.haproxy.enrich_inventory,
             # Depends on kubemarine.core.defaults.apply_registry
             kubemarine.kubernetes.enrich_inventory,
             kubemarine.admission.enrich_inventory,
+            # Depends on kubemarine.core.defaults.apply_defaults
             kubemarine.kubernetes_accounts.enrich_inventory,
             # Depends on kubemarine.kubernetes.enrich_inventory
             kubemarine.cri.enrich_inventory,
             # Depends on kubemarine.core.defaults.apply_registry
             kubemarine.thirdparties.enrich_inventory_apply_defaults,
             # Depends on kubemarine.core.defaults.apply_registry
             kubemarine.plugins.enrich_inventory,
```

### Comparing `kubemarine-0.28.1/kubemarine/core/schema.py` & `kubemarine-0.29.0/kubemarine/core/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,38 +10,57 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
 import pathlib
+from collections.abc import Hashable
 from textwrap import dedent
-from typing import List, Dict, Callable, Union, Sequence, Hashable
+from typing import List, Dict, Callable, Union, Sequence
 
 import jsonschema
 from ordered_set import OrderedSet
 
 from kubemarine.core import utils, log, errors
 from kubemarine.core.cluster import KubernetesCluster, EnrichmentStage, enrichment
 
 
 @enrichment(EnrichmentStage.LIGHT)
+def verify_connections(cluster: KubernetesCluster) -> None:
+    inventory = utils.convert_native_yaml(cluster.inventory)
+    # Run restricted validation of sections that participate in the enrichment of connections.
+    # This is primarily needed for `do`, and `migrate_kubemarine` procedures.
+    _verify_inventory_by_schema(cluster, inventory, 'internal/connections')
+    context = cluster.context
+    args: dict = context['execution_arguments']
+    procedure = context["initial_procedure"]
+    if args.get('procedure_config') and procedure in ('add_node', 'remove_node'):
+        # Run full validation for add_node/remove_node
+        # It is currently not necessary to restrict validation to connections only as for inventory.
+        procedure_inventory = utils.convert_native_yaml(cluster.procedure_inventory)
+        _verify_inventory_by_schema(cluster, procedure_inventory, context["initial_procedure"])
+
+
+@enrichment(EnrichmentStage.FULL)
 def verify_inventory(cluster: KubernetesCluster) -> None:
     inventory = utils.convert_native_yaml(cluster.inventory)
     _verify_inventory_by_schema(cluster, inventory, 'cluster')
     context = cluster.context
     args: dict = context['execution_arguments']
     # Skip validation if procedure inventory is optional and not provided
     if args.get('procedure_config'):
         procedure_inventory = utils.convert_native_yaml(cluster.procedure_inventory)
         _verify_inventory_by_schema(cluster, procedure_inventory, context["initial_procedure"])
 
 
 def _verify_inventory_by_schema(cluster: KubernetesCluster, inventory: dict, schema_name: str) -> None:
-    for_procedure = "" if schema_name == 'cluster' else f" for procedure '{schema_name}'"
+    for_procedure = ("" if schema_name == 'cluster'
+                     else " for connections" if schema_name == 'internal/connections'
+                     else f" for procedure '{schema_name}'")
 
     root_schema_resource = f'resources/schemas/{schema_name}.json'
     root_schema_path = utils.get_internal_resource_path(root_schema_resource)
     root_schema = pathlib.Path(root_schema_path)
     if not root_schema.exists():
         raise Exception(f"Failed to find schema to validate the inventory file{for_procedure}.")
 
@@ -296,36 +315,38 @@
         Failed validating {error.validator!r} in {schema_path}
         On inventory{_convert_to_indices(error.absolute_path)}
         """.rstrip()
     )
 
 
 def _friendly_msg(validator: jsonschema.Draft7Validator, error: jsonschema.ValidationError) -> str:
+    # pylint: disable=too-many-return-statements
+
     if _validated_by(error, 'minProperties'):
         return f"Number of properties is less than the minimum of {error.validator_value!r}. " \
-               f"Property names: {[prop for prop in error.instance]!r}"
+               f"Property names: {list(error.instance)!r}"
 
     if _validated_by(error, 'maxProperties'):
         return f"Number of properties is greater than the maximum of {error.validator_value!r}. " \
-               f"Property names: {[prop for prop in error.instance]!r}"
+               f"Property names: {list(error.instance)!r}"
 
     if _validated_by(error, 'minItems'):
         return f"Number of items equal to {len(error.instance)} is less than the minimum of {error.validator_value!r}"
 
     if _validated_by(error, 'maxItems'):
         return f"Number of items equal to {len(error.instance)} is greater than the maximum of {error.validator_value!r}"
 
     if _validated_by(error, 'type'):
         value = error.validator_value
         expected_types = [value] if isinstance(value, str) else value
         reprs = ", ".join(repr(type) for type in expected_types)
         try:
-            for type in validator.TYPE_CHECKER._type_checkers:
-                if validator.is_type(error.instance, type):  # type: ignore[no-untyped-call]
-                    return f"Actual instance type is {type!r}. Expected: {reprs}."
+            for type_ in validator.TYPE_CHECKER._type_checkers:  # pylint: disable=protected-access
+                if validator.is_type(error.instance, type_):  # type: ignore[no-untyped-call]
+                    return f"Actual instance type is {type_!r}. Expected: {reprs}."
         except (AttributeError, TypeError, jsonschema.exceptions.UnknownType):
             # In current 3rd-party version the error should not appear, but let's still fall back to default behaviour
             pass
 
     if (_validated_by(error, 'not') and isinstance(error.validator_value, dict)
             and set(error.validator_value) == {'enum'} and "propertyNames" in error.schema_path):
         return f"Property name {error.instance!r} is unexpected"
```

### Comparing `kubemarine-0.28.1/kubemarine/core/static.py` & `kubemarine-0.29.0/kubemarine/core/static.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,23 +12,20 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from kubemarine.core import utils
 
 
 def reload() -> None:
-    global GLOBALS
     GLOBALS.clear()
     GLOBALS.update(_load_globals())
 
-    global DEFAULTS
     DEFAULTS.clear()
     DEFAULTS.update(_load_defaults())
 
-    global KUBERNETES_VERSIONS
     KUBERNETES_VERSIONS.clear()
     KUBERNETES_VERSIONS.update(load_kubernetes_versions())
 
 
 def load_compatibility_map(filename: str) -> dict:
     return utils.load_yaml(utils.get_internal_resource_path(
         f"resources/configurations/compatibility/internal/{filename}"))
@@ -38,28 +35,28 @@
     kubernetes_versions = utils.load_yaml(
         utils.get_internal_resource_path('resources/configurations/compatibility/kubernetes_versions.yaml'))
 
     return kubernetes_versions
 
 
 def _load_globals() -> dict:
-    globals = utils.load_yaml(
+    globals_ = utils.load_yaml(
         utils.get_internal_resource_path('resources/configurations/globals.yaml'))
 
     for config_filename in ('kubernetes_images.yaml', 'packages.yaml', 'plugins.yaml', 'thirdparties.yaml'):
         internal_compatibility = load_compatibility_map(config_filename)
 
-        globals_compatibility = globals['compatibility_map']['software']
+        globals_compatibility = globals_['compatibility_map']['software']
         duplicates = set(internal_compatibility) & set(globals_compatibility)
         if duplicates:
             raise Exception(f"Duplicated software {', '.join(repr(s) for s in duplicates)}")
 
         globals_compatibility.update(internal_compatibility)
 
-    return globals
+    return globals_
 
 
 def _load_defaults() -> dict:
     return utils.load_yaml(
         utils.get_internal_resource_path('resources/configurations/defaults.yaml'))
```

### Comparing `kubemarine-0.28.1/kubemarine/core/summary.py` & `kubemarine-0.29.0/kubemarine/core/summary.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,16 +33,16 @@
         self.order = order
         self.text = text
 
     def __lt__(self, other: 'SummaryItem') -> bool:
         return self.order < other.order
 
 
-def schedule_report(context: dict, property: SummaryItem, value: str) -> None:
-    context.setdefault('summary_report', {})[property] = value
+def schedule_report(context: dict, property_: SummaryItem, value: str) -> None:
+    context.setdefault('summary_report', {})[property_] = value
 
 
 def schedule_delayed_report(cluster: KubernetesCluster, call: Callable[[KubernetesCluster], None]) -> None:
     cluster.context.setdefault('delayed_summary_report', []).append(call)
     cluster.schedule_cumulative_point(exec_delayed)
```

### Comparing `kubemarine-0.28.1/kubemarine/core/utils.py` & `kubemarine-0.29.0/kubemarine/core/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,23 +19,23 @@
 import os
 import re
 import shutil
 import sys
 import time
 import tarfile
 import uuid
+from collections import OrderedDict
 from copy import deepcopy
+from datetime import datetime
 
-from typing import Tuple, Callable, List, TextIO, cast, Union, TypeVar, Dict, Sequence, Optional
+from typing import Tuple, Callable, List, TextIO, cast, Union, TypeVar, Dict, Sequence, Optional, NoReturn
 
 import deepdiff  # type: ignore[import-untyped]
 import yaml
 import ruamel.yaml
-from datetime import datetime
-from collections import OrderedDict
 
 from pathvalidate import sanitize_filepath
 from ruamel.yaml import CommentedMap
 from typing_extensions import Protocol
 
 from kubemarine.core import log
 from kubemarine.core.errors import pretty_print_error
@@ -50,15 +50,15 @@
     def __gt__(self, __other: _T_contra) -> bool: ...
 
     def __le__(self, __other: _T_contra) -> bool: ...
 
     def __ge__(self, __other: _T_contra) -> bool: ...
 
 
-def do_fail(message: str = '', reason: Exception = None, hint: str = '', logger: log.EnhancedLogger = None) -> None:
+def do_fail(message: str = '', reason: Exception = None, hint: str = '', logger: log.EnhancedLogger = None) -> NoReturn:
 
     if not logger:
         sys.stderr.write("\033[91m")
 
     pretty_print_error(message, reason, logger)
 
     # Please do not rewrite this to logging approach:
@@ -89,15 +89,15 @@
         shutil.rmtree(dumpdir)
 
     if not args['disable_dump']:
         os.makedirs(dumpdir, exist_ok=True)
 
 
 def make_ansible_inventory(location: str, c: object) -> None:
-    from kubemarine.core.cluster import KubernetesCluster
+    from kubemarine.core.cluster import KubernetesCluster  # pylint: disable=cyclic-import
     cluster = cast(KubernetesCluster, c)
 
     inventory = cluster.inventory
     roles = []
     for node in inventory['nodes']:
         for role in node['roles']:
             if role not in roles:
@@ -134,39 +134,39 @@
             config[role].append(node['name'])
 
     config['cluster:vars'] = [
         'ansible_become=True'
     ]
 
     for group in ['services', 'plugins']:
-        if inventory.get(group) is not None:
-            for service_name, service_configs in inventory[group].items():
-                # write to inventory only plugins, which will be installed
-                if group != 'plugins' or service_configs.get('install', False):
-
-                    config['cluster:vars'].append('\n# %s.%s' % (group, service_name))
-
-                    if isinstance(service_configs, dict):
-
-                        for config_name, config_value in service_configs.items():
-                            if config_name in ('installation', 'install'):
-                                continue
-
-                            if isinstance(config_value, dict) or isinstance(config_value, list):
-                                config_value = json.dumps(config_value)
-                            config['cluster:vars'].append('%s_%s=%s' % (
-                                # TODO: Rewrite replace using regex
-                                service_name.replace('-', '_').replace('.', '_').replace('/', '_'),
-                                config_name.replace('-', '_').replace('.', '_').replace('/', '_'),
-                                config_value))
-                    else:
-                        config_value = json.dumps(service_configs)
-                        config['cluster:vars'].append('%s=%s' % (
-                            service_name.replace('-', '_').replace('.', '_'),
-                            config_value))
+        for service_name, service_configs in inventory.get(group, {}).items():
+            # write to inventory only plugins, which will be installed
+            if group == 'plugins' and not service_configs.get('install', False):
+                continue
+
+            config['cluster:vars'].append('\n# %s.%s' % (group, service_name))
+
+            if isinstance(service_configs, dict):
+
+                for config_name, config_value in service_configs.items():
+                    if config_name in ('installation', 'install'):
+                        continue
+
+                    if isinstance(config_value, (dict, list)):
+                        config_value = json.dumps(config_value)
+                    config['cluster:vars'].append('%s_%s=%s' % (
+                        # TODO: Rewrite replace using regex
+                        service_name.replace('-', '_').replace('.', '_').replace('/', '_'),
+                        config_name.replace('-', '_').replace('.', '_').replace('/', '_'),
+                        config_value))
+            else:
+                config_value = json.dumps(service_configs)
+                config['cluster:vars'].append('%s=%s' % (
+                    service_name.replace('-', '_').replace('.', '_'),
+                    config_value))
 
     config_compiled = ''
     for section_name, strings in config.items():
         config_compiled += '[%s]' % section_name
         for string in strings:
             config_compiled += '\n' + string
         config_compiled += '\n\n'
@@ -205,15 +205,15 @@
 
 
 def dump_file(context: Union[dict, object], data: Union[TextIO, str], filename: str,
               *, dump_location: bool = True) -> None:
     if dump_location:
         if not isinstance(context, dict):
             # cluster is passed instead of the context directly
-            from kubemarine.core.cluster import KubernetesCluster
+            from kubemarine.core.cluster import KubernetesCluster  # pylint: disable=cyclic-import
             cluster = cast(KubernetesCluster, context)
             context = cluster.context
 
         if not is_dump_allowed(context, filename):
             return
 
         target_path = get_dump_filepath(context, filename)
@@ -391,39 +391,43 @@
         buf = io.StringIO()
         yaml_structure_preserver().dump(data, buf)
         data = yaml.safe_load(io.StringIO(buf.getvalue()))
 
     return data
 
 
+def identity(x: str) -> str:
+    return x
+
+
 def is_sorted(l: Sequence[str], key: Callable[[str], SupportsAllComparisons] = None) -> bool:
     """
     Check that the specified list is sorted.
 
     :param l: list to check
     :param key: custom key function to customize the sort order
     :return: boolean flag if the list is sorted
     """
     if key is None:
-        key = lambda x: x
+        key = identity
     return all(key(l[i]) <= key(l[i + 1]) for i in range(len(l) - 1))
 
 
 def map_sorted(map_: CommentedMap, key: Callable[[str], SupportsAllComparisons] = None) -> CommentedMap:
     """
     Check that the specified CommentedMap is sorted, or create new sorted map from it otherwise.
 
     :param map_: CommentedMap instance to check
     :param key: custom key function to customize the sort order of the map keys
     :return: the same or new sorted instance of the map
     """
     if key is not None:
         _key = key
     else:
-        _key = lambda x: x
+        _key = identity
     map_keys: List[str] = list(map_)
     if not is_sorted(map_keys, key=_key):
         map_ = CommentedMap(sorted(map_.items(), key=lambda item: _key(item[0])))
 
     return map_
 
 
@@ -438,15 +442,15 @@
     :param key: custom key function to customize the sort order of the map keys
     """
     if k in map_:
         map_[k] = v
         return
 
     if key is None:
-        key = lambda x: x
+        key = identity
     # Find position to insert new item maintaining the order
     pos = max((mi + 1 for mi, mv in enumerate(map_)
                if key(mv) < key(k)),
               default=0)
 
     map_.insert(pos, k, v)
 
@@ -454,22 +458,20 @@
 def load_yaml(filepath: str) -> dict:
     try:
         with open_utf8(filepath, 'r') as stream:
             data: dict = yaml.safe_load(stream)
             return data
     except yaml.YAMLError as exc:
         do_fail(f"Failed to load {filepath}", exc)
-        return {}  # unreachable
 
 
 def strtobool(value: Union[str, bool]) -> bool:
     """
     The method check string and boolean value
     :param value: Value that should be checked
-    :param section: inventory section for debugging purpose
     """
     val = str(value).lower()
     if val in ('y', 'yes', 't', 'true', 'on', '1'):
         return True
     elif val in ('n', 'no', 'f', 'false', 'off', '0'):
         return False
     else:
@@ -480,15 +482,15 @@
     if isinstance(value, int):
         return value
 
     try:
         # whitespace required because python's int() ignores them
         return int(value.replace(' ', '.'))
     except ValueError:
-        raise ValueError(f"invalid integer value {value!r}")
+        raise ValueError(f"invalid integer value {value!r}") from None
 
 
 def print_diff(logger: log.EnhancedLogger, diff: deepdiff.DeepDiff) -> None:
     # Extra transformation to JSON is necessary,
     # because DeepDiff.to_dict() returns custom nested classes that cannot be serialized to yaml by default.
     logger.debug(yaml.safe_dump(yaml.safe_load(diff.to_json())))
 
@@ -633,15 +635,15 @@
     4- Copying dumps to new nodes
     """
 
     PRESERVED_DUMP_FILES = ['procedure.yaml', 'procedure_parameters',
                             'cluster.yaml', 'cluster_initial.yaml', 'cluster_finalized.yaml']
 
     def __init__(self, cluster: object, context: dict):
-        from kubemarine.core.cluster import KubernetesCluster
+        from kubemarine.core.cluster import KubernetesCluster  # pylint: disable=cyclic-import
         self.cluster = cast(KubernetesCluster, cluster)
         self.context = context
         self.dir_path = "/etc/kubemarine/procedures/"
         self.dir_location = ''
         self.local_archive_path = ''
 
     def make_dir(self) -> None:
@@ -676,42 +678,46 @@
         node_group_results = control_planes.sudo(command)
         with control_planes.new_executor() as exe:
             for control_plane in exe.group.get_ordered_members_list():
                 result = node_group_results[control_plane.get_host()]
                 files = result.stdout.split()
                 files.sort(reverse=True)
                 for i, file in enumerate(files):
-                    if i >= not_pack_file and i < delete_old:
+                    if not_pack_file <= i < delete_old:
                         if 'tar.gz' not in file:
                             control_plane.sudo(
                                 f'tar -czvf {self.dir_path + file + ".tar.gz"} {self.dir_path + file} &&'
                                 f'sudo rm -r {self.dir_path + file}')
                     elif i >= delete_old:
                         control_plane.sudo(f'rm -rf {self.dir_path + file}')
 
-    def compress_archive(self) -> None:
+    def compress_archive(self, enriched: bool) -> None:
         """
         This method compose dump files in the local archive.
         """
         context = self.context
         self.local_archive_path = get_dump_filepath(context, "local.tar.gz")
         with tarfile.open(self.local_archive_path, "w:gz") as tar:
-            for name in ClusterStorage.PRESERVED_DUMP_FILES:
+            dump_files = set(ClusterStorage.PRESERVED_DUMP_FILES)
+            if not enriched:
+                dump_files -= {'cluster.yaml', 'cluster_finalized.yaml'}
+
+            for name in dump_files:
                 source = get_dump_filepath(context, name)
                 if os.path.exists(source):
                     tar.add(source, 'dump/' + name)
             tar.add(context['execution_arguments']['config'], 'cluster.yaml')
             tar.add(get_version_filepath(), 'version')
 
     def collect_procedure_info(self) -> None:
         """
         This method collects information about the type of procedure and the version of the tool we are working with.
         """
         context = self.context
-        out = dict()
+        out = {}
         out['arguments'] = context['initial_cli_arguments']
         if 'proceeded_tasks' in context:
             out['finished_tasks'] = context['proceeded_tasks']
         out["initial_procedure"] = context["initial_procedure"]
         out["successfully_performed"] = context["successfully_performed"]
         out['status'] = context['status']
         output = yaml.dump(out)
```

### Comparing `kubemarine-0.28.1/kubemarine/core/yaml_merger.py` & `kubemarine-0.29.0/kubemarine/core/yaml_merger.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from deepmerge import Merger  # type: ignore[import-untyped]
 
 
 def is_list_extends(nxt: list) -> bool:
     return any({'<<': 'merge'} == v for i, v in enumerate(nxt))
 
 
-def list_merger(config: Merger, path: list, base: list, nxt: list) -> list:
+def list_merger(_: Merger, path: list, base: list, nxt: list) -> list:
     strategy = None
     strategy_definition_position = 0
     for i, v in enumerate(nxt):
         if isinstance(v, dict) and '<<' in v:
             if strategy is not None:
                 raise Exception(f"Found more than one merge strategy definitions at path {path}.")
             strategy = v.get('<<')
```

### Comparing `kubemarine-0.28.1/kubemarine/coredns.py` & `kubemarine-0.29.0/kubemarine/coredns.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,23 +7,22 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import io
 from typing import Union, List, Optional, Any, Dict, Tuple
 
 import yaml
 
 from kubemarine import system
 from kubemarine.core import utils
 
-import io
-
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.core.group import RunnersGroupResult
 
 
 def proceed_section_keyvalue(data: Dict[str, Any], tabsize: int) -> str:
     tab = " "*tabsize
     config = ''
@@ -48,15 +47,15 @@
             config += generate_nested_sections(key, value, tabsize)
             continue
         raise Exception('Unknown type of field in coredns services')
 
     return config
 
 
-def generate_nested_sections(type: str, data: Dict[str, Dict[str, Any]], tabsize: int) -> str:
+def generate_nested_sections(type_: str, data: Dict[str, Dict[str, Any]], tabsize: int) -> str:
     tab = " "*tabsize
     config = ''
 
     max_priority = 0
     for section_name, section_value in data.items():
         if section_value.get('priority') is not None and section_value['priority'] > max_priority:
             max_priority = section_value['priority']
@@ -74,46 +73,46 @@
             sections.append((section_name, section_priority))
 
     sections = sorted(sections, key=lambda i: i[1])
 
     for section in sections:
         section_name, _ = section
         section_value = data[section_name]
-        if type == 'kubernetes':
-            config += '\n' + tab + type
+        if type_ == 'kubernetes':
+            config += '\n' + tab + type_
             if section_value.get('zone'):
                 if isinstance(section_value['zone'], list):
                     section_value['zone'] = ' '.join(section_value['zone'])
                 config += ' ' + section_value['zone']
             config += ' {' + proceed_section_keyvalue(section_value['data'], tabsize + 2) + '\n' + tab + '}'
 
-        elif type == 'hosts':
-            config += '\n' + tab + type
+        elif type_ == 'hosts':
+            config += '\n' + tab + type_
             if section_value.get('file') and isinstance(section_value['file'], str):
                 config += ' ' + section_value['file']
             config += ' {' + proceed_section_keyvalue(section_value['data'], tabsize + 2) + '\n' + tab + '}'
 
-        elif type == 'template':
+        elif type_ == 'template':
             zones: Union[str, List[Optional[str]]] = [None]
             if section_value.get('zone'):
                 zones = section_value['zone']
                 if isinstance(zones, str):
                     zones = [zones]
             for zone in zones:
-                config += '\n' + tab + type
+                config += '\n' + tab + type_
                 if section_value.get('class'):
                     config += ' ' + section_value['class']
                 if section_value.get('type'):
                     config += ' ' + section_value['type']
                 if zone:
                     config += ' ' + zone
                 config += ' {' + proceed_section_keyvalue(section_value['data'], tabsize + 2) + '\n' + tab + '}'
 
         else:
-            config += '\n' + tab + type + ' {' + proceed_section_keyvalue(section_value['data'], tabsize + 2)\
+            config += '\n' + tab + type_ + ' {' + proceed_section_keyvalue(section_value['data'], tabsize + 2) \
                       + '\n' + tab + '}'
 
     return config
 
 
 def generate_configmap(inventory: dict) -> str:
     # coredns.configmap.Hosts must exist even if it's empty
@@ -145,15 +144,15 @@
 
     return config + '\n'
 
 
 def apply_configmap(cluster: KubernetesCluster, config: str) -> RunnersGroupResult:
     utils.dump_file(cluster, config, 'coredns-configmap.yaml')
 
-    group = cluster.make_group_from_roles(['control-plane', 'worker'])
+    group = cluster.make_group_from_roles(['control-plane'])
     group.put(io.StringIO(config), '/etc/kubernetes/coredns-configmap.yaml', backup=True, sudo=True)
 
     return cluster.nodes['control-plane'].get_first_member()\
         .sudo('kubectl apply -f /etc/kubernetes/coredns-configmap.yaml && '
              'sudo kubectl rollout restart -n kube-system deployment/coredns')
 
 
@@ -170,15 +169,15 @@
 
         config = yaml.dump(cluster.inventory['services']['coredns'][config_type])
         filename = 'coredns-%s-patch.yaml' % config_type
         filepath = '/etc/kubernetes/' + filename
 
         utils.dump_file(cluster, config, filename)
 
-        group = cluster.make_group_from_roles(['control-plane', 'worker'])
+        group = cluster.make_group_from_roles(['control-plane'])
         group.put(io.StringIO(config), filepath, backup=True, sudo=True)
 
         apply_command = 'kubectl patch %s coredns -n kube-system --type merge -p \"$(sudo cat %s)\"' % (config_type, filepath)
 
     if apply_command == '':
         return 'Nothing to patch'
```

### Comparing `kubemarine-0.28.1/kubemarine/cri/__init__.py` & `kubemarine-0.29.0/kubemarine/cri/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/cri/containerd.py` & `kubemarine-0.29.0/kubemarine/cri/containerd.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import base64
 from io import StringIO
 from typing import Dict, List, Tuple, Optional
 
 import toml
 import yaml
-import base64
 
 from kubemarine import system, packages, jinja
 from kubemarine.core import utils, static, errors
 from kubemarine.core.cluster import KubernetesCluster, EnrichmentStage, enrichment
 from kubemarine.core.group import NodeGroup, RunnersGroupResult, CollectorCallback
 from kubemarine.core.yaml_merger import default_merger
 
@@ -139,16 +139,18 @@
                         != get_sandbox_image(cluster.inventory['services']['cri']))
 
     cluster.context.setdefault("upgrade", {}).setdefault('required', {})['containerdConfig'] = upgrade_required
 
 
 @enrichment(EnrichmentStage.PROCEDURE, procedures=['migrate_cri'])
 def enrich_migrate_cri_inventory(cluster: KubernetesCluster) -> None:
-    if cluster.previous_inventory["services"]["cri"]["containerRuntime"] == cluster.procedure_inventory["cri"]["containerRuntime"]:
-        raise Exception("You already have such cri or you should explicitly specify 'cri.containerRuntime: docker' in cluster.yaml")
+    if (cluster.previous_inventory["services"]["cri"]["containerRuntime"]
+            == cluster.procedure_inventory["cri"]["containerRuntime"]):
+        raise Exception("You already have such cri "
+                        "or you should explicitly specify 'cri.containerRuntime: docker' in cluster.yaml")
 
     cri_section = cluster.inventory.setdefault("services", {}).setdefault("cri", {})
 
     if cri_section.get("dockerConfig", {}):
         del cri_section["dockerConfig"]
 
     default_merger.merge(cri_section, utils.deepcopy_yaml(cluster.procedure_inventory["cri"]))
```

### Comparing `kubemarine-0.28.1/kubemarine/cri/docker.py` & `kubemarine-0.29.0/kubemarine/cri/docker.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/demo.py` & `kubemarine-0.29.0/kubemarine/demo.py`

 * *Files 3% similar despite different names*

```diff
@@ -180,32 +180,29 @@
         result = {}
         for host in hosts:
             result[host] = self.read(host, filename)
         return result
 
 
 class FakeClusterStorage(utils.ClusterStorage):
-    def __init__(self, cluster: object, context: dict):
-        super().__init__(cluster, context)
-
     def make_dir(self) -> None:
         pass
 
     def upload_and_rotate(self) -> None:
         cluster = cast(FakeKubernetesCluster, self.cluster)
         cluster.uploaded_archives.append(self.local_archive_path)
 
     def upload_info_new_control_planes(self) -> None:
         pass
 
 
 class FakeKubernetesCluster(KubernetesCluster):
 
     def __init__(self, *args: Any, **kwargs: Any):
-        self.resources: FakeResources = kwargs.pop("resources")
+        self.resources: FakeClusterResources = kwargs.pop("resources")
         self.fake_shell = self.resources.fake_shell
         self.fake_fs = self.resources.fake_fs
         self.uploaded_archives: List[str] = []
         super().__init__(*args, **kwargs)
 
     def _create_connection_pool(self, nodes: Dict[str, dict], gateway_nodes: Dict[str, dict], hosts: List[str]) -> ConnectionPool:
         return FakeConnectionPool(nodes, gateway_nodes, hosts, self.fake_shell, self.fake_fs)
@@ -213,28 +210,24 @@
     def _create_cluster_storage(self, context: dict) -> utils.ClusterStorage:
         return FakeClusterStorage(self, context)
 
     def make_group(self, ips: Iterable[_AnyConnectionTypes]) -> FakeNodeGroup:
         return FakeNodeGroup(ips, self)
 
 
-class FakeResources(DynamicResources):
-    def __init__(self, context: dict, inventory: dict = None, procedure_inventory: dict = None,
+class FakeClusterResources(DynamicResources):
+    def __init__(self, context: dict,
+                 *,
                  nodes_context: Dict[str, Any] = None,
-                 fake_shell: FakeShell = None, fake_fs: FakeFS = None, make_finalized_inventory: Optional[bool] = False):
+                 fake_shell: FakeShell = None, fake_fs: FakeFS = None):
         super().__init__(context)
-        self.inventory_filepath = None
-        self.procedure_inventory_filepath = None
         self.fake_shell = fake_shell if fake_shell else FakeShell()
         self.fake_fs = fake_fs if fake_fs else FakeFS()
-        self._inventory = inventory
-        self._procedure_inventory = procedure_inventory
 
         self.finalized_inventory: dict = {}
-        self.make_finalized_inventory = make_finalized_inventory
 
         self._enrichment_functions = super().enrichment_functions()
         # Let's do not assign self._nodes_context directly to make it more close to the real enrichment.
         if nodes_context is not None:
             fn_idx = self._enrichment_functions.index(system.detect_nodes_context)
             self._enrichment_functions[fn_idx] = enrichment(EnrichmentStage.LIGHT)\
                 (lambda c: c.nodes_context.update(nodes_context))
@@ -243,26 +236,21 @@
     def working_inventory(self) -> dict:
         cluster = self.cluster_if_initialized()
         if cluster is not None:
             return cluster.inventory
 
         return {}
 
-    def _store_inventory(self, inventory: dict) -> None:
-        pass
-
-    def _make_finalized_inventory(self, finalized_filename: str) -> bool:
-        if self.make_finalized_inventory is None:
-            return super()._make_finalized_inventory(finalized_filename)
-
-        return self.make_finalized_inventory
-
     def _store_finalized_inventory(self, finalized_inventory: dict, finalized_filename: str) -> None:
         self.finalized_inventory = finalized_inventory
-        utils.dump_file(self, yaml.dump(finalized_inventory), finalized_filename)
+        super()._store_finalized_inventory(finalized_inventory, finalized_filename)
+
+    def cluster_if_initialized(self) -> Optional[FakeKubernetesCluster]:
+        cluster = super().cluster_if_initialized()
+        return None if cluster is None else cast(FakeKubernetesCluster, cluster)
 
     def cluster(self, stage: EnrichmentStage = EnrichmentStage.PROCEDURE) -> FakeKubernetesCluster:
         return cast(FakeKubernetesCluster, super().cluster(stage))
 
     def _new_cluster_instance(self, context: dict) -> FakeKubernetesCluster:
         return FakeKubernetesCluster(
             self.inventory(), context, self.procedure_inventory(),
@@ -286,14 +274,34 @@
 
         self._skip_default_enrichment = None
 
     def enrichment_functions(self) -> List[EnrichmentFunction]:
         return self._enrichment_functions
 
 
+class FakeResources(FakeClusterResources):
+    def __init__(self, context: dict, inventory: dict = None,
+                 *,
+                 procedure_inventory: dict = None,
+                 nodes_context: Dict[str, Any] = None,
+                 fake_shell: FakeShell = None, fake_fs: FakeFS = None):
+        super().__init__(context, nodes_context=nodes_context, fake_shell=fake_shell, fake_fs=fake_fs)
+        self.inventory_filepath = None
+        self.procedure_inventory_filepath = None
+        self._inventory = inventory
+        self._procedure_inventory = procedure_inventory
+
+    def _store_inventory(self, inventory: dict) -> None:
+        pass
+
+    def _store_finalized_inventory(self, finalized_inventory: dict, finalized_filename: str) -> None:
+        self.finalized_inventory = finalized_inventory
+        utils.dump_file(self, yaml.dump(finalized_inventory), finalized_filename)
+
+
 class FakeConnection(fabric.connection.Connection):  # type: ignore[misc]
 
     def __init__(self, ip: str, fake_shell: FakeShell, fake_fs: FakeFS, **kw: Any):
         super().__init__(ip, **kw)
         self.fake_shell = fake_shell
         self.fake_fs = fake_fs
 
@@ -314,18 +322,18 @@
     def run(self, command: str, **kwargs: Any) -> fabric.runners.Result:
         return self._do("run", command, **kwargs)
 
     def sudo(self, command: str, **kwargs: Any) -> fabric.runners.Result:
         return self._do("sudo", command, **kwargs)
 
     # not implemented
-    def get(self, remote_file: str, local_file: str, **kwargs: Any) -> None:
+    def get(self, remote_file: str, local_file: str, **kwargs: Any) -> None:  # pylint: disable=arguments-differ
         raise NotImplementedError("Stub for fabric Connection.get() is not implemented")
 
-    def put(self, data: Union[io.BytesIO, str], filename: str, **kwargs: Any) -> None:
+    def put(self, data: Union[io.BytesIO, str], filename: str, **kwargs: Any) -> None:  # pylint: disable=arguments-differ
         # It should return fabric.transfer.Result, but currently returns None.
         # Transfer Result is currently never handled.
         self.fake_fs.write(self.host, filename, data)
 
     def _do(self, do_type: str, original_command: str, **kwargs: Any) -> fabric.runners.Result:
         # start fake execution of commands
         commands, sep_symbol, command_sep = self._split_command(do_type, original_command)
@@ -446,26 +454,27 @@
         self.fake_fs = fake_fs
         super().__init__(nodes, gateway_nodes, hosts)
 
     def _create_connection_from_details(self, ip: str, conn_details: dict,
                                         gateway: fabric.connection.Connection = None,
                                         inline_ssh_env: bool = True) -> fabric.connection.Connection:
         return FakeConnection(
-            ip, self.fake_shell, self.fake_fs,
+            ip, self.fake_shell, self.fake_fs, gateway=gateway,
             user=conn_details.get('username', static.GLOBALS['connection']['defaults']['username']),
             port=conn_details.get('connection_port', static.GLOBALS['connection']['defaults']['port'])
         )
 
 
 def create_silent_context(args: list = None, procedure: str = 'install') -> dict:
     args = list(args) if args else []
     # todo probably increase logging level to get rid of spam in logs.
 
     context: dict = procedures.import_procedure(procedure).create_context(args)
     context['preserve_inventory'] = False
+    context['make_finalized_inventory'] = False
     context['load_inventory_silent'] = True
 
     parsed_args: dict = context['execution_arguments']
     parsed_args['disable_dump'] = True
     del parsed_args['ansible_inventory_location']
 
     return context
@@ -557,17 +566,15 @@
             'cri': {}
         },
         'cluster_name': 'k8s.fake.local'
     }
 
     id_roles_map: Dict[str, List[str]] = {}
 
-    for role_name in ['balancer', 'master', 'worker']:
-
-        item = locals()[role_name]
+    for role_name, item in (('balancer', balancer), ('master', master), ('worker', worker)):
 
         if isinstance(item, int):
             ids = []
             if item > 0:
                 for i in range(0, item):
                     ids.append('%s-%s' % (role_name, i + 1))
             item = ids
```

### Comparing `kubemarine-0.28.1/kubemarine/etcd.py` & `kubemarine-0.29.0/kubemarine/etcd.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,19 +81,19 @@
             if etcd_health.get('health'):
                 health += 1
 
         if health == len(etcd_health_list):
             log.debug('All ETCD members are healthy!')
             is_healthy = True
             break
-        else:
-            log.debug('Wait for ETCD cluster is not healthy!')
-            if sudo_time < timeout:
-                time.sleep(timeout - sudo_time)
-            retries -= 1
+
+        log.debug('Wait for ETCD cluster is not healthy!')
+        if sudo_time < timeout:
+            time.sleep(timeout - sudo_time)
+        retries -= 1
 
     if is_healthy:
         etcd_status_raw = connection.sudo('etcdctl endpoint status --cluster -w json').get_simple_out()
         log.verbose(etcd_status_raw)
         etcd_status_list: List[dict] = json.load(io.StringIO(etcd_status_raw.lower().strip()))
         elected_leader: Optional[int] = None
         for item in etcd_status_list:
```

### Comparing `kubemarine-0.28.1/kubemarine/haproxy.py` & `kubemarine-0.29.0/kubemarine/haproxy.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/jinja.py` & `kubemarine-0.29.0/kubemarine/jinja.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,19 +16,24 @@
 from urllib.parse import quote_plus
 
 import yaml
 import jinja2
 
 from kubemarine.core import log, utils
 
+FILTER = Callable[[str], Any]
+
 
 def new(_: log.EnhancedLogger, *,
         recursive_compiler: Callable[[str], str] = None,
-        precompile_filters: Dict[str, Callable[[str], Any]] = None) -> jinja2.Environment:
-    def _precompile(filter_: str, struct: str) -> str:
+        precompile_filters: Dict[str, FILTER] = None) -> jinja2.Environment:
+    def _precompile(filter_: str, struct: str, *args: Any, **kwargs: Any) -> str:
+        if args or kwargs:
+            raise ValueError(f"Filter {filter_!r} does not support extra arguments")
+
         if not isinstance(struct, str):
             raise ValueError(f"Filter {filter_!r} can be applied only on string")
 
         # maybe we have non compiled string like templates/plugins/calico-{{ globals.compatibility_map }} ?
         return recursive_compiler(struct) if recursive_compiler is not None and is_template(struct) else struct
 
     env = jinja2.Environment()
@@ -37,18 +42,21 @@
         precompile_filters = {}
     precompile_filters['isipv4'] = lambda ip: utils.isipv(ip, [4])
     precompile_filters['minorversion'] = utils.minor_version
     precompile_filters['majorversion'] = utils.major_version
     precompile_filters['versionkey'] = utils.version_key
     precompile_filters['b64encode'] = lambda s: base64.b64encode(s.encode()).decode()
     precompile_filters['b64decode'] = lambda s: base64.b64decode(s.encode()).decode()
-    precompile_filters['url_quote'] = lambda u: quote_plus(u)
+    precompile_filters['url_quote'] = quote_plus
 
     for name, filter_ in precompile_filters.items():
-        env.filters[name] = lambda s, n=name, f=filter_: f(_precompile(n, s))
+        def make_filter(n: str, f: FILTER) -> FILTER:
+            return lambda s, *args, **kwargs: f(_precompile(n, s, *args, *kwargs))
+
+        env.filters[name] = make_filter(name, filter_)
 
     env.filters['toyaml'] = lambda data: yaml.dump(data, default_flow_style=False)
     env.tests['has_role'] = lambda node, role: role in node['roles']
     env.tests['has_roles'] = lambda node, roles: bool(set(node['roles']) & set(roles))
 
     # we need these filters because rendered cluster.yaml can contain variables like 
     # enable: 'true'
```

### Comparing `kubemarine-0.28.1/kubemarine/k8s_certs.py` & `kubemarine-0.29.0/kubemarine/k8s_certs.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/keepalived.py` & `kubemarine-0.29.0/kubemarine/keepalived.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,19 +120,19 @@
                 record['priority'] = priority_settings['max_value'] - (j + priority_settings['step'])
             if not record.get('interface') and item.get('interface'):
                 record['interface'] = item['interface']
             if record.get('interface', 'auto') == 'auto':
                 record['interface'] = autodetect_interface(cluster, record['name'])
 
 
-def get_all_balancer_names(inventory: dict, *, final: bool = True) -> List[str]:
+def get_all_balancer_names(inventory: dict) -> List[str]:
     default_names = []
 
     # well, vrrp_ips is not empty, let's find balancers defined in config-file
-    for i, node in enumerate(inventory['nodes']):
+    for node in inventory['nodes']:
         if 'balancer' in node['roles']:
             default_names.append(node['name'])
 
     return default_names
 
 
 @enrichment(EnrichmentStage.FULL)
@@ -142,15 +142,15 @@
     # if vrrp_ips is empty, then nothing to do
     if not inventory['vrrp_ips']:
         return
 
     # Calculate group, where keepalived should be installed:
     names = []
 
-    for i, item in enumerate(inventory['vrrp_ips']):
+    for item in inventory['vrrp_ips']:
         for record in item['hosts']:
             names.append(record['name'])
 
     # Create new group from balancers with Keepalived (to be) on them.
     keepalived_group = cluster.make_group_from_roles(['balancer']).new_group(apply_filter={
         'name': names
     })
```

### Comparing `kubemarine-0.28.1/kubemarine/kubernetes/__init__.py` & `kubemarine-0.29.0/kubemarine/kubernetes/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 import os
 import time
 from contextlib import contextmanager
 from typing import List, Dict, Iterator, Any, Optional
 
 import yaml
 from jinja2 import Template
-import ipaddress
 
 from kubemarine import system, admission, etcd, packages, jinja
 from kubemarine.core import utils, static, summary, log, errors
 from kubemarine.core.cluster import KubernetesCluster, EnrichmentStage, enrichment
 from kubemarine.core.executor import Token
 from kubemarine.core.group import NodeGroup, DeferredGroup, RunnersGroupResult, CollectorCallback
 from kubemarine.core.errors import KME
@@ -180,15 +179,16 @@
     # check ignorePreflightErrors value and add mandatory errors from defaults.yaml if they're absent
     default_preflight_errors = static.DEFAULTS["services"]["kubeadm_flags"]["ignorePreflightErrors"].split(",")
     preflight_errors = inventory["services"]["kubeadm_flags"]["ignorePreflightErrors"].split(",")
 
     preflight_errors.extend(default_preflight_errors)
     inventory["services"]["kubeadm_flags"]["ignorePreflightErrors"] = ",".join(set(preflight_errors))
 
-    # override kubeadm_kube-proxy.conntrack.min with sysctl.net.netfilter.nf_conntrack_max since they define the same kernel variable
+    # override kubeadm_kube-proxy.conntrack.min with sysctl.net.netfilter.nf_conntrack_max
+    # since they define the same kernel variable
     version_key = utils.version_key(inventory["services"]["kubeadm"]["kubernetesVersion"])
     conntrack_max = inventory["services"]["sysctl"].get("net.netfilter.nf_conntrack_max")
     if version_key >= (1, 29, 0) and conntrack_max is not None:
         inventory["services"]["kubeadm_kube-proxy"]["conntrack"]["min"] = conntrack_max
     else:
         inventory["services"]["kubeadm_kube-proxy"]["conntrack"].pop("min",None)
 
@@ -271,15 +271,19 @@
     result = control_plane.sudo("kubectl get nodes -o custom-columns=NAME:.metadata.name")
 
     stdout = list(result.values())[0].stdout
     log.verbose("Detected the following nodes in cluster:\n%s" % stdout)
 
     for node in group.get_ordered_members_list():
         node_name = node.get_node_name()
-        if node_name in stdout:
+
+        # Split stdout into lines
+        stdout_lines = stdout.split('\n')[1:]
+        # Check if node_name exactly matches any line
+        if node_name in stdout_lines:
             log.debug("Draining node %s..." % node_name)
             drain_cmd = prepare_drain_command(
                 cluster, node_name,
                 disable_eviction=disable_eviction, drain_timeout=drain_timeout, grace_period=grace_period)
             control_plane.sudo(drain_cmd, hide=False)
         else:
             log.warning("Node %s is not found in cluster and can't be drained" % node_name)
@@ -295,15 +299,19 @@
     result = control_plane.sudo("kubectl get nodes -o custom-columns=NAME:.metadata.name")
 
     stdout = list(result.values())[0].stdout
     log.verbose("Detected the following nodes in cluster:\n%s" % stdout)
 
     for node in group.get_ordered_members_list():
         node_name = node.get_node_name()
-        if node_name in stdout:
+        
+        # Split stdout into lines
+        stdout_lines = stdout.split('\n')[1:]
+        # Check if node_name exactly matches any line
+        if node_name in stdout_lines:
             log.debug("Deleting node %s from the cluster..." % node_name)
             control_plane.sudo("kubectl delete node %s" % node_name, hide=False)
         else:
             log.warning("Node %s is not found in cluster and can't be removed" % node_name)
 
     return control_plane.sudo("kubectl get nodes")
 
@@ -389,15 +397,15 @@
 
     cluster_name = nodes.cluster.inventory['cluster_name']
 
     try:
         with nodes.new_executor() as exe:
             for defer in exe.group.get_ordered_members_list():
                 internal_address = defer.get_config()['internal_address']
-                if type(ipaddress.ip_address(internal_address)) is ipaddress.IPv6Address:
+                if utils.isipv(internal_address, [6]):
                     internal_address = f"[{internal_address}]"
 
                 defer.sudo(
                     f"cp /root/.kube/config {temp_filepath} "
                     f"&& sudo sed -i 's/{cluster_name}/{internal_address}/' {temp_filepath}")
         yield temp_filepath
     finally:
@@ -417,15 +425,15 @@
     log.debug(f"Downloading kubeconfig from node {first_control_plane.get_node_name()!r}...")
 
     kubeconfig = list(first_control_plane.sudo('cat /root/.kube/config').values())[0].stdout
 
     # Replace cluster FQDN with ip
     public_cluster_ip = cluster.inventory.get('public_cluster_ip')
     if public_cluster_ip:
-        if type(ipaddress.ip_address(public_cluster_ip)) is ipaddress.IPv6Address:
+        if utils.isipv(public_cluster_ip, [6]):
             public_cluster_ip = f"[{public_cluster_ip}]"
         cluster_name = cluster.inventory['cluster_name']
         kubeconfig = kubeconfig.replace(cluster_name, public_cluster_ip)
 
     kubeconfig_filename = os.path.abspath("kubeconfig")
     utils.dump_file(cluster.context, kubeconfig, kubeconfig_filename, dump_location=False)
     cluster.log.debug(f"Kubeconfig saved to {kubeconfig_filename}")
@@ -571,15 +579,17 @@
         if correct_conditions == len(wait_conditions):
             log.debug("All nodes are ready!")
             return
         else:
             retries = retries - 1
             time.sleep(timeout)
 
-    raise Exception("Nodes did not become ready in the expected time, %s retries every %s seconds. Try to increase node.ready.retries parameter in globals: https://github.com/Netcracker/KubeMarine/blob/main/documentation/Installation.md#globals" % (retries, timeout))
+    raise Exception(f"Nodes did not become ready in the expected time, {retries} retries every {timeout} seconds. "
+                    "Try to increase node.ready.retries parameter in globals: "
+                    "https://github.com/Netcracker/KubeMarine/blob/main/documentation/Installation.md#globals")
 
 
 def init_workers(group: NodeGroup) -> None:
     if group.is_empty():
         return
 
     cluster: KubernetesCluster = group.cluster
@@ -681,15 +691,17 @@
         return
 
     cluster.log.debug("Upgrading first control-plane \"%s\"" % node_name)
 
     # put control-plane patches
     components.create_kubeadm_patches_for_node(cluster, first_control_plane)
 
-    flags = "-f --certificate-renewal=true --ignore-preflight-errors='%s' --patches=/etc/kubernetes/patches" % cluster.inventory['services']['kubeadm_flags']['ignorePreflightErrors']
+    flags = ("-f --certificate-renewal=true "
+             f"--ignore-preflight-errors='{cluster.inventory['services']['kubeadm_flags']['ignorePreflightErrors']}' "
+             f"--patches=/etc/kubernetes/patches")
 
     drain_cmd = prepare_drain_command(cluster, node_name, **drain_kwargs)
     first_control_plane.sudo(drain_cmd, hide=False)
 
     upgrade_cri_if_required(first_control_plane)
     fix_flag_kubelet(first_control_plane)
 
@@ -1121,17 +1133,17 @@
             if role in actual_roles[name]:
                 members += 1
                 conditions = nodes_conditions[name]
                 if conditions.get('Ready', {}).get('status') == 'True' \
                         and conditions.get('NetworkUnavailable', {}).get('status') == 'False':
                     ready += 1
 
-        property = summary.SummaryItem.CONTROL_PLANES if role == 'control-plane' else summary.SummaryItem.WORKERS
+        property_ = summary.SummaryItem.CONTROL_PLANES if role == 'control-plane' else summary.SummaryItem.WORKERS
         value = f'{ready}/{members}'
-        summary.schedule_report(cluster.context, property, value)
+        summary.schedule_report(cluster.context, property_, value)
 
 
 def get_nodes_description_cmd() -> str:
     return 'kubectl get node -o yaml'
 
 
 def get_nodes_description(cluster: KubernetesCluster) -> dict:
```

### Comparing `kubemarine-0.28.1/kubemarine/kubernetes/components.py` & `kubemarine-0.29.0/kubemarine/kubernetes/components.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/kubernetes/daemonset.py` & `kubemarine-0.29.0/kubemarine/kubernetes/daemonset.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/kubernetes/deployment.py` & `kubemarine-0.29.0/kubemarine/kubernetes/deployment.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/kubernetes/object.py` & `kubemarine-0.29.0/kubemarine/kubernetes/object.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/kubernetes/replicaset.py` & `kubemarine-0.29.0/kubemarine/kubernetes/replicaset.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/kubernetes/secrets.py` & `kubemarine-0.29.0/kubemarine/kubernetes/secrets.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/kubernetes/statefulset.py` & `kubemarine-0.29.0/kubemarine/kubernetes/statefulset.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/kubernetes_accounts.py` & `kubemarine-0.29.0/kubemarine/kubernetes_accounts.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,16 @@
                 rbac["accounts"][i]['configs'].pop(2)
             if rbac["accounts"][i]['configs'][0].get('secrets') is not None:
                 rbac["accounts"][i]['configs'][0].pop('secrets')
         else:
            # This part is applicable for Kubernetes v1.24 and higher
            # It has 'Secret' in addition 
             if account['configs'][2]['metadata'].get('name') is None:
-                rbac["accounts"][i]['configs'][2]['metadata']['annotations']['kubernetes.io/service-account.name'] = account['name']
+                rbac["accounts"][i]['configs'][2]['metadata']['annotations']['kubernetes.io/service-account.name'] \
+                    = account['name']
                 rbac["accounts"][i]['configs'][2]['metadata']['name'] = f"{account['name']}-token"
                 rbac["accounts"][i]['configs'][0]['secrets'].append({})
                 rbac["accounts"][i]['configs'][0]['secrets'][0]['name'] = f"{account['name']}-token"
             if account['configs'][2]['metadata'].get('namespace') is None:
                 rbac["accounts"][i]['configs'][2]['metadata']['namespace'] = account['namespace']
```

### Comparing `kubemarine-0.28.1/kubemarine/modprobe.py` & `kubemarine-0.29.0/kubemarine/modprobe.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/packages.py` & `kubemarine-0.29.0/kubemarine/packages.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import re
 from typing import List, Dict, Tuple, Optional, Union, Mapping, Set
 
 from typing_extensions import Protocol
 
 from kubemarine import yum, apt, jinja
 from kubemarine.core import errors, static, utils
 from kubemarine.core.cluster import KubernetesCluster, EnrichmentStage, enrichment
@@ -284,15 +285,17 @@
     os_family = different_os[0][0]
     if os_family in ('unknown', 'unsupported'):
         # For add_node/install procedures we check that OS is supported in prepare.check.system task.
         # For check_iaas procedure it is allowed to have unsupported OS, so skip caching.
         cluster.log.debug("Skip caching of packages for unsupported OS.")
         return inventory
 
-    group = (cluster.previous_nodes if by_initial_nodes else cluster.nodes)['all']
+    group = (cluster.previous_nodes if by_initial_nodes else cluster.nodes)['all'] \
+        .exclude_group(cluster.nodes['all'].get_online_nodes(False))
+
     if group.nodes_amount() != group.get_sudo_nodes().nodes_amount():
         # For add_node/install procedures we check that all nodes are sudoers in prepare.check.sudoer task.
         # For check_iaas procedure the nodes might still be not sudoers.
         # Skip caching if any not-sudoer node found.
         cluster.log.debug(f"Some nodes are not sudoers, packages will not be cached.")
         return inventory
 
@@ -645,16 +648,14 @@
 
 
 def get_package_name(os_family: str, package: str) -> str:
     """
     Return the pure package name, without any part of version
     """
 
-    import re
-
     package_name = ""
 
     if package:
         if os_family in ["rhel", "rhel8", "rhel9"]:
             # regexp is needed to split package and its version, the pattern start with '-' then should be number or '*'
             package_name = re.split(r'-[\d,\*]', package)[0]
         else:
```

### Comparing `kubemarine-0.28.1/kubemarine/patches/__init__.py` & `kubemarine-0.29.0/kubemarine/resources/etalons/patches/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,16 +18,14 @@
 
 The whole directory is automatically cleared and reset after new version of Kubemarine is released.
 """
 
 from typing import List
 
 from kubemarine.core.patch import Patch
-from kubemarine.patches.patch_kubelet_configmap import KubeletResolvConf
 
 patches: List[Patch] = [
-    KubeletResolvConf(),
 ]
 """
 List of patches that is sorted according to the Patch.priority() before execution.
 Patches that have the same priority, are executed in the declared order.
 """
```

### Comparing `kubemarine-0.28.1/kubemarine/patches/patch_kubelet_configmap.py` & `kubemarine-0.29.0/kubemarine/patches/strong_cipher_suits_for_kubelet.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,51 +9,35 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from textwrap import dedent
-
 from kubemarine.core.action import Action
 from kubemarine.core.patch import RegularPatch
 from kubemarine.core.resources import DynamicResources
-from kubemarine.kubernetes import components
-
+from kubemarine.kubernetes.components import reconfigure_components
 
 class TheAction(Action):
     def __init__(self) -> None:
-        super().__init__("Remove default resolvConf from kubelet-config ConfigMap")
+        super().__init__("Update kubelet TLS cipher suites (if necessary)")
 
     def run(self, res: DynamicResources) -> None:
-        cluster = res.cluster()
-        control_plane = cluster.nodes['control-plane'].get_first_member()
-
-        kubeadm_config = components.KubeadmConfig(cluster)
-        if 'resolvConf' in kubeadm_config.maps['kubelet-config']:
-            return cluster.log.info("KubeletConfiguration.resolvConf is redefined in the inventory. "
-                                    "Patch is not applicable.")
-
-        if 'resolvConf' not in kubeadm_config.load('kubelet-config', control_plane):
-            return cluster.log.info("KubeletConfiguration.resolvConf is already absent in the kubelet-config ConfigMap.")
-
-        control_plane.call(components.patch_kubelet_configmap)
-
+        kubernetes_nodes = res.cluster().make_group_from_roles(['control-plane', 'worker'])
+        reconfigure_components(kubernetes_nodes, ['kubelet'])
 
-class KubeletResolvConf(RegularPatch):
+class UpdatekubeletCipherSuites(RegularPatch):
     def __init__(self) -> None:
-        super().__init__("kubelet_resolvConf")
+        super().__init__("kubelet_cipher_suites")
 
     @property
     def action(self) -> Action:
         return TheAction()
 
     @property
     def description(self) -> str:
         return dedent(
             f"""\
-            If KubeletConfiguration.resolvConf is not redefined in the inventory,
-            remove it from the kubelet-config ConfigMap if present.
-            
-            This is necessary for smoother migration of the operating systems.
+            Patch to update the kubelet TLS cipher suites.
             """.rstrip()
-        )
+        )
```

### Comparing `kubemarine-0.28.1/kubemarine/patches/software_upgrade.yaml` & `kubemarine-0.29.0/kubemarine/resources/etalons/patches/software_upgrade.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/plugins/__init__.py` & `kubemarine-0.29.0/kubemarine/plugins/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import glob
 import importlib.util
+import inspect
 import io
 import os
 import re
 import shutil
 import ssl
 import subprocess
 import sys
@@ -27,15 +28,14 @@
 import urllib.request
 import zipfile
 from itertools import chain
 from types import ModuleType, FunctionType
 from typing import Dict, List, Tuple, Callable, Union, no_type_check, Set, Any, cast, TextIO, Optional
 
 import yaml
-import inspect
 
 from kubemarine.core.cluster import KubernetesCluster, EnrichmentStage, enrichment
 from kubemarine import jinja, thirdparties
 from kubemarine.core import utils, static, errors, os as kos, log
 from kubemarine.core.yaml_merger import default_merger
 from kubemarine.core.group import NodeGroup
 from kubemarine.kubernetes.daemonset import DaemonSet
@@ -69,15 +69,15 @@
         # The following section rewrites DEFAULT plugins registries
         # and does not touch user-defined registries in plugins
         for plugin_name, plugin_item in cluster.inventory['plugins'].items():
             if cluster.raw_inventory.get('plugins', {}).get(plugin_name, {}).get('installation', {}).get('registry') is None:
                 plugin_item.setdefault('installation', {})['registry'] = plugins_default_registry
 
     for plugin_name, plugin_item in inventory["plugins"].items():
-        for i, step in enumerate(plugin_item.get('installation', {}).get('procedures', [])):
+        for step in plugin_item.get('installation', {}).get('procedures', []):
             for procedure_type, configs in step.items():
                 if procedure_types()[procedure_type].get('convert') is not None:
                     step[procedure_type] = procedure_types()[procedure_type]['convert'](cluster, configs)
 
 
 def _get_upgrade_plan(cluster: KubernetesCluster) -> List[Tuple[str, dict]]:
     context = cluster.context
@@ -202,15 +202,15 @@
     for plugin_name in plugins_queue:
         install_plugin(cluster, plugin_name, plugins[plugin_name]["installation"]['procedures'])
 
 
 def install_plugin(cluster: KubernetesCluster, plugin_name: str, installation_procedure: List[dict]) -> None:
     cluster.log.debug("**** INSTALLING PLUGIN %s ****" % plugin_name)
 
-    for current_step_i, step in enumerate(installation_procedure):
+    for step in installation_procedure:
         for apply_type, configs in step.items():
             procedure_types()[apply_type]['apply'](cluster, configs)
 
 
 def expect_daemonset(cluster: KubernetesCluster,
                      daemonsets_names: List[Union[str, Dict[str, str]]],
                      timeout: int = None,
@@ -256,15 +256,18 @@
             cluster.log.debug("DaemonSets are up to date")
             return
         else:
             retries -= 1
             cluster.log.debug(f"DaemonSets are not up to date yet... ({retries * timeout}s left)")
             time.sleep(timeout)
 
-    raise Exception('In the expected time, the DaemonSets did not become ready. Try to increase number of retries in expect.daemonsets: https://github.com/Netcracker/KubeMarine/blob/main/documentation/Installation.md#expect-deploymentsdaemonsetsreplicasetsstatefulsets')
+    raise Exception('In the expected time, the DaemonSets did not become ready. '
+                    'Try to increase number of retries in expect.daemonsets: '
+                    # pylint: disable-next=line-too-long
+                    'https://github.com/Netcracker/KubeMarine/blob/main/documentation/Installation.md#expect-deploymentsdaemonsetsreplicasetsstatefulsets')
 
 
 def expect_replicaset(cluster: KubernetesCluster,
                       replicasets_names: List[Union[str, Dict[str, str]]],
                       timeout: int = None,
                       retries: int = None,
                       node: NodeGroup = None) -> None:
@@ -308,15 +311,18 @@
             cluster.log.debug("ReplicaSets are up to date")
             return
         else:
             retries -= 1
             cluster.log.debug(f"ReplicaSets are not up to date yet... ({retries * timeout}s left)")
             time.sleep(timeout)
 
-    raise Exception('In the expected time, the ReplicaSets did not become ready. Try to increase number of retries in expect.replicasets: https://github.com/Netcracker/KubeMarine/blob/main/documentation/Installation.md#expect-deploymentsdaemonsetsreplicasetsstatefulsets')
+    raise Exception('In the expected time, the ReplicaSets did not become ready. '
+                    'Try to increase number of retries in expect.replicasets: '
+                    # pylint: disable-next=line-too-long
+                    'https://github.com/Netcracker/KubeMarine/blob/main/documentation/Installation.md#expect-deploymentsdaemonsetsreplicasetsstatefulsets')
 
 
 def expect_statefulset(cluster: KubernetesCluster,
                        statefulsets_names: List[Union[str, Dict[str, str]]],
                        timeout: int = None,
                        retries: int = None,
                        node: NodeGroup = None) -> None:
@@ -360,15 +366,18 @@
             cluster.log.debug("StatefulSets are up to date")
             return
         else:
             retries -= 1
             cluster.log.debug(f"StatefulSets are not up to date yet... ({retries * timeout}s left)")
             time.sleep(timeout)
 
-    raise Exception('In the expected time, the StatefulSets did not become ready. Try to increase number of retries in expect.statefulsets: https://github.com/Netcracker/KubeMarine/blob/main/documentation/Installation.md#expect-deploymentsdaemonsetsreplicasetsstatefulsets')
+    raise Exception('In the expected time, the StatefulSets did not become ready. '
+                    'Try to increase number of retries in expect.statefulsets: '
+                    # pylint: disable-next=line-too-long
+                    'https://github.com/Netcracker/KubeMarine/blob/main/documentation/Installation.md#expect-deploymentsdaemonsetsreplicasetsstatefulsets')
 
 
 def expect_deployment(cluster: KubernetesCluster,
                       deployments_names: List[Union[str, Dict[str, str]]],
                       timeout: int = None,
                       retries: int = None,
                       node: NodeGroup = None) -> None:
@@ -412,15 +421,18 @@
             cluster.log.debug("Deployments are up to date!")
             return
         else:
             retries -= 1
             cluster.log.debug(f"Deployments are not up to date yet... ({retries * timeout}s left)")
             time.sleep(timeout)
 
-    raise Exception('In the expected time, the Deployments did not become ready. Try to increase number of retries in expect.deployments: https://github.com/Netcracker/KubeMarine/blob/main/documentation/Installation.md#expect-deploymentsdaemonsetsreplicasetsstatefulsets')
+    raise Exception('In the expected time, the Deployments did not become ready. '
+                    'Try to increase number of retries in expect.deployments: '
+                    # pylint: disable-next=line-too-long
+                    'https://github.com/Netcracker/KubeMarine/blob/main/documentation/Installation.md#expect-deploymentsdaemonsetsreplicasetsstatefulsets')
 
 
 def expect_pods(cluster: KubernetesCluster, pods: List[str], namespace: str = None,
                 timeout: int = None, retries: int = None,
                 control_plane: NodeGroup = None, node_name: str = None) -> None:
 
     if timeout is None:
@@ -510,15 +522,15 @@
 
 # **** TEMPLATES ****
 
 def convert_template(_: KubernetesCluster, config: Union[str, dict]) -> dict:
     return _convert_file(config)
 
 
-def verify_template(_: KubernetesCluster, config: dict, plugin_name: Optional[str] = None) -> None:
+def verify_template(_: KubernetesCluster, config: dict, _plugin_name: Optional[str] = None) -> None:
     _verify_file(config, "Template")
 
 
 def apply_template(cluster: KubernetesCluster, config: dict) -> None:
     _apply_file(cluster, config, "Template")
 
 
@@ -547,15 +559,15 @@
         }
     return config
 
 
 def apply_expect(cluster: KubernetesCluster, config: dict) -> None:
     # TODO: Add support for expect services and expect nodes
 
-    for expect_type, expect_conf in config.items():
+    for expect_type in config:
         if expect_type == 'daemonsets':
             expect_daemonset(cluster, config['daemonsets']['list'],
                              timeout=config['daemonsets'].get('timeout'),
                              retries=config['daemonsets'].get('retries'))
 
         elif expect_type == 'replicasets':
             expect_replicaset(cluster, config['replicasets']['list'],
@@ -587,15 +599,15 @@
 
     spec = importlib.util.spec_from_file_location('module', module_path)
     try:
         module = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(module)
         LOADED_MODULES[module_path] = module
     except Exception as e:
-        raise ValueError(f"Could not import module {module_path}: {e}")
+        raise ValueError(f"Could not import module {module_path}: {e}") from None
     return module 
 
 
 def get_python_method_args(step: dict) -> Tuple[str, FunctionType, Dict[str, Any]]:
     module_path, _ = utils.determine_resource_absolute_file(step['module'])
     method_name = step['method']
     method_arguments = step.get('arguments', {})
@@ -618,26 +630,27 @@
     # Get the signature of the method
     signature = inspect.signature(method)
 
     # Check if the passed arguments match the signature
     try:
         signature.bind(cluster, **method_arguments)
     except TypeError as e:
-        raise ValueError(f"Invalid arguments for python method {method.__name__} for {plugin_name!r} plugin: {e}")
+        raise ValueError(f"Invalid arguments for python method {method.__name__} for {plugin_name!r} plugin: {e}") \
+            from None
 
 
 def apply_python(cluster: KubernetesCluster, step: dict) -> None:
     module_path, method, method_arguments = get_python_method_args(step)
     cluster.log.debug("Running method %s from %s module..." % (method.__name__, module_path))
     method(cluster, **method_arguments)
 
 
 # **** THIRDPARTIES ****
 
-def verify_thirdparty(cluster: KubernetesCluster, thirdparty: str, plugin_name: Optional[str] = None) -> None:
+def verify_thirdparty(cluster: KubernetesCluster, thirdparty: str, _plugin_name: Optional[str] = None) -> None:
     defined_thirdparties = list(cluster.inventory['services'].get('thirdparties', {}).keys())
     if thirdparty not in defined_thirdparties:
         raise Exception('Specified thirdparty %s not found in thirdpartirs definition. Expected any of %s.'
                         % (thirdparty, defined_thirdparties))
 
 
 def apply_thirdparty(cluster: KubernetesCluster, thirdparty: str) -> None:
@@ -650,15 +663,15 @@
     if isinstance(config, str):
         config = {
             'command': config
         }
     return config
 
 
-def verify_shell(cluster: KubernetesCluster, config: dict, plugin_name: Optional[str] = None) -> None:
+def verify_shell(cluster: KubernetesCluster, config: dict, _plugin_name: Optional[str] = None) -> None:
     out_vars = config.get('out_vars', [])
     groups = config.get('groups', [])
     nodes = config.get('nodes', [])
     explicit_group = cluster.create_group_from_groups_nodes_names(groups, nodes)
     if out_vars and (groups or nodes) and explicit_group.nodes_amount() != 1:
         raise Exception('Shell output variables could be used for single-node groups, but multi-node group was found')
 
@@ -745,15 +758,15 @@
     return config
 
 
 def _get_absolute_playbook(config: dict) -> str:
     return utils.determine_resource_absolute_file(config['playbook'])[0]
 
 
-def verify_ansible(cluster: KubernetesCluster, config: dict, plugin_name: Optional[str] = None) -> None:
+def verify_ansible(cluster: KubernetesCluster, config: dict, _plugin_name: Optional[str] = None) -> None:
     _get_absolute_playbook(config)
     if cluster.is_deploying_from_windows():
         raise Exception("Executing of playbooks on Windows deployer is currently not supported")
     # TODO: verify fields types and contents
 
 
 def apply_ansible(cluster: KubernetesCluster, step: dict) -> None:
@@ -776,24 +789,24 @@
         _vars = []
         for k, v in external_vars.items():
             _vars.append('%s=%s' % (k, v))
         command += ' --extra-vars "%s"' % ' '.join(_vars)
 
     cluster.log.verbose("Running shell \"%s\"" % command)
 
-    result = subprocess.run(command, stdout=sys.stdout, stderr=sys.stderr, shell=True)
+    result = subprocess.run(command, stdout=sys.stdout, stderr=sys.stderr, shell=True, check=False)
     if result.returncode != 0:
         raise Exception("Failed to apply ansible plugin, see error above")
 
 
 def apply_helm(cluster: KubernetesCluster, config: dict) -> None:
     chart_path = get_local_chart_path(cluster.log, config)
     process_chart_values(config, chart_path)
 
-    from kubemarine import kubernetes
+    from kubemarine import kubernetes  # pylint: disable=cyclic-import
     local_config_path = kubernetes.fetch_admin_config(cluster)
 
     with utils.open_external(os.path.join(chart_path, 'Chart.yaml'), 'r') as stream:
         chart_metadata = yaml.safe_load(stream)
         chart_name = chart_metadata["name"]
 
     cluster.log.debug("Running helm chart %s" % chart_name)
@@ -933,15 +946,15 @@
     return local_chart_folder
 
 
 def convert_config(_: KubernetesCluster, config: Union[str, dict]) -> dict:
     return _convert_file(config)
 
 
-def verify_config(_: KubernetesCluster, config: dict, plugin_name: Optional[str] = None) -> None:
+def verify_config(_: KubernetesCluster, config: dict, _plugin_name: Optional[str] = None) -> None:
     _verify_file(config, "Config")
 
 
 def apply_config(cluster: KubernetesCluster, config: dict) -> None:
     _apply_file(cluster, config, "Config")
```

### Comparing `kubemarine-0.28.1/kubemarine/plugins/builtin.py` & `kubemarine-0.29.0/kubemarine/plugins/builtin.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/plugins/calico.py` & `kubemarine-0.29.0/kubemarine/plugins/calico.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,22 +7,21 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import ipaddress
 from textwrap import dedent
 from typing import Optional, List, Dict
 
 import os
 import yaml
 
-from kubemarine import plugins, kubernetes
+from kubemarine import plugins
 from kubemarine.core import utils, log
 from kubemarine.core.cluster import KubernetesCluster, EnrichmentStage, enrichment
 from kubemarine.core.group import NodeGroup
 from kubemarine.kubernetes import secrets
 from kubemarine.plugins.manifest import Processor, EnrichmentFunction, Manifest, Identity
 
 
@@ -112,14 +111,16 @@
 
 def is_apiserver_enabled(inventory: dict) -> bool:
     enabled: bool = inventory['plugins']['calico']['apiserver']['enabled']
     return enabled
 
 
 def renew_apiserver_certificate(cluster: KubernetesCluster) -> None:
+    from kubemarine import kubernetes  # pylint: disable=cyclic-import
+
     logger = cluster.log
     if not is_apiserver_enabled(cluster.inventory):
         logger.debug("Calico API server is disabled. Skip renewing of the key and certificate.")
         return
 
     namespace = "calico-apiserver"
     secret_name = "calico-apiserver-certs"
@@ -197,28 +198,29 @@
         source_yaml['data']['veth_mtu'] = str(val)
         self.log.verbose(f"The {key} has been patched in 'data.veth_mtu' with '{val}'")
         val = "calico-typha" if is_typha_enabled(self.inventory) else "none"
         source_yaml['data']['typha_service_name'] = val
         self.log.verbose(f"The {key} has been patched in 'data.typha_service_name' with '{val}'")
         string_part = source_yaml['data']['cni_network_config']
         ip = self.inventory['services']['kubeadm']['networking']['podSubnet'].split('/')[0]
-        if type(ipaddress.ip_address(ip)) is ipaddress.IPv4Address:
+        if utils.isipv(ip, [4]):
             val = self.inventory['plugins']['calico']['cni']['ipam']['ipv4']
         else:
             val = self.inventory['plugins']['calico']['cni']['ipam']['ipv6']
         new_string_part = string_part.replace('"type": "calico-ipam"', str(val)[:-1][1:].replace("'", "\""))
         source_yaml['data']['cni_network_config'] = new_string_part
         log_str = new_string_part.replace("\n", "")
         self.log.verbose(f"The {key} has been patched in 'data.cni_network_config' with '{log_str}'")
 
     def enrich_service_account_secret_calico_kube_controllers(self, manifest: Manifest) -> None:
         new_yaml = yaml.safe_load(service_account_secret_calico_kube_controllers)
 
         service_account_key = "ServiceAccount_calico-kube-controllers"
-        service_account_index = manifest.all_obj_keys().index(service_account_key) if service_account_key in manifest.all_obj_keys() else -1
+        service_account_index = manifest.all_obj_keys().index(service_account_key) \
+            if service_account_key in manifest.all_obj_keys() else -1
         
         self.include(manifest, service_account_index + 1, new_yaml)
 
     def enrich_service_account_calico_kube_controllers(self, manifest: Manifest) -> None:
         key = "ServiceAccount_calico-kube-controllers"
         source_yaml = manifest.get_obj(key, patch=True)
         source_yaml['automountServiceAccountToken'] = False
@@ -240,15 +242,16 @@
         self.enrich_image_for_container(manifest, key,
             plugin_service='kube-controllers', container_name='calico-kube-controllers', is_init_container=False)
 
     def enrich_service_account_secret_calico_node(self, manifest: Manifest) -> None:
         new_yaml = yaml.safe_load(service_account_secret_calico_node)
 
         service_account_key = "ServiceAccount_calico-node"
-        service_account_index = manifest.all_obj_keys().index(service_account_key) if service_account_key in manifest.all_obj_keys() else -1
+        service_account_index = manifest.all_obj_keys().index(service_account_key) \
+            if service_account_key in manifest.all_obj_keys() else -1
         
         self.include(manifest, service_account_index + 1, new_yaml)
 
     def enrich_service_account_calico_node(self, manifest: Manifest) -> None:
         key = "ServiceAccount_calico-node"
         source_yaml = manifest.get_obj(key, patch=True)
         source_yaml['automountServiceAccountToken'] = False
@@ -288,15 +291,15 @@
         The method attempts to preserve initial formatting.
 
         :param manifest: Container to operate with manifest objects
         """
         key = "DaemonSet_calico-node"
         env_delete: List[str] = []
         ip = self.inventory['services']['kubeadm']['networking']['podSubnet'].split('/')[0]
-        if type(ipaddress.ip_address(ip)) is ipaddress.IPv4Address:
+        if utils.isipv(ip, [4]):
             env_delete.extend([
                 'CALICO_IPV6POOL_CIDR', 'IP6', 'IP6_AUTODETECTION_METHOD',
                 'CALICO_IPV6POOL_IPIP', 'CALICO_IPV6POOL_VXLAN'
             ])
         if not is_typha_enabled(self.inventory):
             env_delete.append('FELIX_TYPHAK8SSERVICENAME')
 
@@ -518,15 +521,16 @@
     def enrich_namespace_calico_apiserver(self, manifest: Manifest) -> None:
         self.assign_default_pss_labels(manifest, 'calico-apiserver')
 
     def enrich_service_account_secret_calico_apiserver(self, manifest: Manifest) -> None:
         new_yaml = yaml.safe_load(service_account_secret_calico_apiserver)
 
         service_account_key = "ServiceAccount_calico-apiserver"
-        service_account_index = manifest.all_obj_keys().index(service_account_key) if service_account_key in manifest.all_obj_keys() else -1
+        service_account_index = manifest.all_obj_keys().index(service_account_key) \
+            if service_account_key in manifest.all_obj_keys() else -1
         
         self.include(manifest, service_account_index + 1, new_yaml)
 
     def enrich_service_account_calico_apiserver(self, manifest: Manifest) -> None:
         key = "ServiceAccount_calico-apiserver"
         source_yaml = manifest.get_obj(key, patch=True)
         source_yaml['automountServiceAccountToken'] = False
```

### Comparing `kubemarine-0.28.1/kubemarine/plugins/kubernetes_dashboard.py` & `kubemarine-0.29.0/kubemarine/plugins/kubernetes_dashboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from textwrap import dedent
 from typing import List, Optional, Dict
 import yaml
-from textwrap import dedent
 
 from kubemarine.core import summary, utils, log
 from kubemarine.core.cluster import KubernetesCluster, EnrichmentStage, enrichment
 from kubemarine.plugins.manifest import Processor, EnrichmentFunction, Manifest, Identity
 
 
 @enrichment(EnrichmentStage.FULL)
@@ -80,15 +80,16 @@
     def enrich_namespace_kubernetes_dashboard(self, manifest: Manifest) -> None:
         self.assign_default_pss_labels(manifest, 'kubernetes-dashboard')
 
     def enrich_service_account_secret_kubernetes_dashboard(self, manifest: Manifest) -> None:
         new_yaml = yaml.safe_load(service_account_secret_kubernetes_dashboard)
 
         service_account_key = "ServiceAccount_kubernetes-dashboard"
-        service_account_index = manifest.all_obj_keys().index(service_account_key) if service_account_key in manifest.all_obj_keys() else -1
+        service_account_index = manifest.all_obj_keys().index(service_account_key) \
+            if service_account_key in manifest.all_obj_keys() else -1
         
         self.include(manifest, service_account_index + 1, new_yaml)
 
     def enrich_service_account_kubernetes_dashboard(self, manifest: Manifest) -> None:
         key = "ServiceAccount_kubernetes-dashboard"
         source_yaml = manifest.get_obj(key, patch=True)
         source_yaml['automountServiceAccountToken'] = False
@@ -117,15 +118,16 @@
         self.enrich_volume_and_volumemount(source_yaml, service_account_name)
        
         self.log.verbose(f"The {key} has been updated to include the new secret volume and mount.")
 
         self.enrich_image_for_container(manifest, key,
             plugin_service='metrics-scraper', container_name='dashboard-metrics-scraper', is_init_container=False)
 
-        self.enrich_resources_for_container(manifest, key, container_name='dashboard-metrics-scraper', plugin_service="metrics-scraper")
+        self.enrich_resources_for_container(
+            manifest, key, container_name='dashboard-metrics-scraper', plugin_service="metrics-scraper")
         self.enrich_node_selector(manifest, key, plugin_service='metrics-scraper')
         self.enrich_tolerations(manifest, key, plugin_service='metrics-scraper', override=True)
 
 
 class V2_5_X_DashboardManifestProcessor(DashboardManifestProcessor):
     def enrich_deployment_dashboard_metrics_scraper(self, manifest: Manifest) -> None:
         key = "Deployment_dashboard-metrics-scraper"
```

### Comparing `kubemarine-0.28.1/kubemarine/plugins/local_path_provisioner.py` & `kubemarine-0.29.0/kubemarine/plugins/local_path_provisioner.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,16 @@
     def enrich_namespace_local_path_storage(self, manifest: Manifest) -> None:
         self.assign_default_pss_labels(manifest, 'local-path-storage')
 
     def enrich_service_account_secret(self, manifest: Manifest) -> None:
         new_yaml = yaml.safe_load(service_account_secret)
 
         service_account_key = "ServiceAccount_local-path-provisioner-service-account"
-        service_account_index = manifest.all_obj_keys().index(service_account_key) if service_account_key in manifest.all_obj_keys() else -1
+        service_account_index = manifest.all_obj_keys().index(service_account_key) \
+            if service_account_key in manifest.all_obj_keys() else -1
         
         self.include(manifest, service_account_index + 1, new_yaml)
 
     def add_clusterrolebinding_local_path_provisioner_privileged_psp(self, manifest: Manifest) -> None:
         # TODO add only if psp is enabled?
         new_yaml = yaml.safe_load(clusterrolebinding_local_path_provisioner_privileged_psp)
         # Insert new ClusterRoleBinding after all existing resources of this kind
```

### Comparing `kubemarine-0.28.1/kubemarine/plugins/manifest.py` & `kubemarine-0.29.0/kubemarine/plugins/manifest.py`

 * *Files 2% similar despite different names*

```diff
@@ -302,15 +302,15 @@
 
         return f'{self.manifest_identity.name}-{self.get_version()}.yaml'
 
     def assign_default_pss_labels(self, manifest: Manifest, namespace: str) -> None:
         key = f"Namespace_{namespace}"
         rbac = self.inventory['rbac']
         if rbac['admission'] == 'pss' and rbac['pss']['pod-security'] == 'enabled':
-            from kubemarine import admission
+            from kubemarine import admission  # pylint: disable=cyclic-import
 
             profile = self.get_namespace_to_necessary_pss_profiles()[namespace]
             target_labels = admission.get_labels_to_ensure_profile(self.inventory, profile)
             if not target_labels:
                 return
 
             source_yaml = manifest.get_obj(key, patch=True)
@@ -453,15 +453,16 @@
 
         plugin_service_section = self.inventory['plugins'][self.plugin_name]
         if plugin_service:
             plugin_service_section = plugin_service_section[plugin_service]
         container['resources'] = plugin_service_section['resources']
 
         self.log.verbose(f"The {key} has been patched in "
-                         f"'spec.template.spec.containers.[{container_pos}].resources' with {plugin_service_section['resources']!r}")
+                         f"'spec.template.spec.containers.[{container_pos}].resources' "
+                         f"with {plugin_service_section['resources']!r}")
 
     def enrich_args_for_container(self, manifest: Manifest, key: str,
                                   *,
                                   plugin_service: str,
                                   container_name: str,
                                   remove_args: List[str] = None,
                                   extra_args: List[str] = None) -> None:
@@ -503,18 +504,18 @@
         for extra_arg in extra_args:
             extra_arg_key = extra_arg.split('=')[0]
             for i, container_arg in enumerate(container_args):
                 if container_arg == extra_arg_key or container_arg.startswith(extra_arg_key + "="):
                     raise Exception(
                         f"{extra_arg_key!r} argument is already defined in "
                         f"'spec.template.spec.containers.[{container_pos}].args' for the {key}.")
-            else:
-                container_args.append(extra_arg)
-                self.log.verbose(f"The {extra_arg!r} argument has been added to "
-                                 f"'spec.template.spec.containers.[{container_pos}].args' in the {key}")
+
+            container_args.append(extra_arg)
+            self.log.verbose(f"The {extra_arg!r} argument has been added to "
+                             f"'spec.template.spec.containers.[{container_pos}].args' in the {key}")
 
     def enrich_env_for_container(self, manifest: Manifest, key: str,
                                  *,
                                  plugin_service: Optional[str] = None,
                                  container_name: str,
                                  env_delete: List[str] = None,
                                  env_ensure: Mapping[str, Union[str, dict]] = None) -> None:
@@ -544,17 +545,17 @@
                     self.log.verbose(f"The {name!r} env variable has been removed from "
                                      f"'spec.template.spec.containers.[{container_pos}].env' in the {key}")
                     break
 
         env_update: Dict[str, dict] = {}
 
         def update_env(name: str, value: Union[str, dict]) -> None:
-            if type(value) is str:
+            if isinstance(value, str):
                 env_update[name] = {'value': value}
-            elif type(value) is dict:
+            elif isinstance(value, dict):
                 env_update[name] = {'valueFrom': value}
             self.log.verbose(f"The {key} has been patched in "
                              f"'spec.template.spec.containers.[{container_pos}].env.{name}' with '{value}'")
 
         if env_ensure is None:
             env_ensure = {}
 
@@ -575,17 +576,17 @@
         for env in container['env']:
             name = env['name']
             if name not in env_update:
                 continue
 
             value = env_update.pop(name)
             keys = list(env.keys())
-            for key in keys:
-                if key != 'name' and key not in value:
-                    del env[key]
+            for k in keys:
+                if k != 'name' and k not in value:
+                    del env[k]
 
             env.update(value)
 
         for name, env in env_update.items():
             new_env = {'name' : name}
             new_env.update(env)
             container['env'].append(new_env)
```

### Comparing `kubemarine-0.28.1/kubemarine/plugins/nginx_ingress.py` & `kubemarine-0.29.0/kubemarine/plugins/nginx_ingress.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import io
-import ipaddress
 from typing import Optional, List, Dict
 
 from textwrap import dedent
 import yaml
 
 from kubemarine.core import utils, log
 from kubemarine.core.cluster import KubernetesCluster, EnrichmentStage, enrichment
@@ -198,15 +197,16 @@
             self.log.verbose(f"The {manifest.obj_key(custom_headers_cm)} has been patched in 'data' "
                              f"with the data from 'plugins.nginx-ingress-controller.custom_headers'")
             
     def enrich_service_account_secret(self, manifest: Manifest) -> None:
         new_yaml = yaml.safe_load(service_account_secret)
 
         service_account_key = "ServiceAccount_ingress-nginx"
-        service_account_index = manifest.all_obj_keys().index(service_account_key) if service_account_key in manifest.all_obj_keys() else -1
+        service_account_index = manifest.all_obj_keys().index(service_account_key) \
+            if service_account_key in manifest.all_obj_keys() else -1
         
         self.include(manifest, service_account_index + 1, new_yaml)
 
     def enrich_service_account(self, manifest: Manifest) -> None:
         key = "ServiceAccount_ingress-nginx"
         source_yaml = manifest.get_obj(key, patch=True)
         source_yaml['automountServiceAccountToken'] = False
@@ -287,15 +287,15 @@
 
         self.enrich_resources_for_container(manifest, key, container_name='patch', plugin_service="webhook")
 
     def enrich_service_ingress_nginx_controller(self, manifest: Manifest) -> None:
         # The method needs some rework in case of dual stack support
         key = "Service_ingress-nginx-controller"
         ip = self.inventory['services']['kubeadm']['networking']['serviceSubnet'].split('/')[0]
-        if type(ipaddress.ip_address(ip)) is ipaddress.IPv6Address:
+        if utils.isipv(ip, [6]):
             source_yaml = manifest.get_obj(key, patch=True)
             source_yaml['spec']['ipFamilies'] = ['IPv6']
             self.log.verbose(f"The {key} has been patched in 'spec.ipFamilies' with 'IPv6'")
 
 
 class V1_2_X_IngressNginxManifestProcessor(IngressNginxManifestProcessor):
     def get_enrichment_functions(self) -> List[EnrichmentFunction]:
```

### Comparing `kubemarine-0.28.1/kubemarine/plugins/yaml/calico-apiserver-v3.24.2-original.yaml` & `kubemarine-0.29.0/kubemarine/plugins/yaml/calico-apiserver-v3.24.2-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/plugins/yaml/calico-apiserver-v3.25.1-original.yaml` & `kubemarine-0.29.0/kubemarine/plugins/yaml/calico-apiserver-v3.25.1-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/plugins/yaml/calico-apiserver-v3.26.1-original.yaml` & `kubemarine-0.29.0/kubemarine/plugins/yaml/calico-apiserver-v3.26.1-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/plugins/yaml/calico-apiserver-v3.26.4-original.yaml` & `kubemarine-0.29.0/kubemarine/plugins/yaml/calico-apiserver-v3.26.4-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/plugins/yaml/calico-apiserver-v3.27.0-original.yaml` & `kubemarine-0.29.0/kubemarine/plugins/yaml/calico-apiserver-v3.27.0-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/plugins/yaml/calico-v3.22.2-original.yaml` & `kubemarine-0.29.0/kubemarine/plugins/yaml/calico-v3.22.2-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/plugins/yaml/calico-v3.24.2-original.yaml` & `kubemarine-0.29.0/kubemarine/plugins/yaml/calico-v3.24.2-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/plugins/yaml/calico-v3.25.1-original.yaml` & `kubemarine-0.29.0/kubemarine/plugins/yaml/calico-v3.25.1-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/plugins/yaml/calico-v3.26.1-original.yaml` & `kubemarine-0.29.0/kubemarine/plugins/yaml/calico-v3.26.1-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/plugins/yaml/calico-v3.26.4-original.yaml` & `kubemarine-0.29.0/kubemarine/plugins/yaml/calico-v3.26.4-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/plugins/yaml/calico-v3.27.0-original.yaml` & `kubemarine-0.29.0/kubemarine/plugins/yaml/calico-v3.27.0-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/plugins/yaml/kubernetes-dashboard-v2.5.1-original.yaml` & `kubemarine-0.29.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.5.1-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/plugins/yaml/kubernetes-dashboard-v2.7.0-original.yaml` & `kubemarine-0.29.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.7.0-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/plugins/yaml/local-path-provisioner-v0.0.22-original.yaml` & `kubemarine-0.29.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.22-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/plugins/yaml/local-path-provisioner-v0.0.23-original.yaml` & `kubemarine-0.29.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.23-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/plugins/yaml/local-path-provisioner-v0.0.24-original.yaml` & `kubemarine-0.29.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.24-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/plugins/yaml/local-path-provisioner-v0.0.25-original.yaml` & `kubemarine-0.29.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.25-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/plugins/yaml/local-path-provisioner-v0.0.26-original.yaml` & `kubemarine-0.29.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.26-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/plugins/yaml/nginx-ingress-controller-v1.2.0-original.yaml` & `kubemarine-0.29.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.2.0-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/plugins/yaml/nginx-ingress-controller-v1.4.0-original.yaml` & `kubemarine-0.29.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.4.0-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/plugins/yaml/nginx-ingress-controller-v1.7.0-original.yaml` & `kubemarine-0.29.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.7.0-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/plugins/yaml/nginx-ingress-controller-v1.8.1-original.yaml` & `kubemarine-0.29.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.8.1-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/plugins/yaml/nginx-ingress-controller-v1.8.4-original.yaml` & `kubemarine-0.29.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.8.4-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/plugins/yaml/nginx-ingress-controller-v1.9.4-original.yaml` & `kubemarine-0.29.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.9.4-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/plugins/yaml/nginx-ingress-controller-v1.9.5-original.yaml` & `kubemarine-0.29.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.9.5-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/procedures/__init__.py` & `kubemarine-0.29.0/kubemarine/procedures/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/procedures/add_node.py` & `kubemarine-0.29.0/kubemarine/procedures/add_node.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/procedures/backup.py` & `kubemarine-0.29.0/kubemarine/procedures/backup.py`

 * *Files 0% similar despite different names*

```diff
@@ -543,15 +543,15 @@
                 temp_local_filepath = os.path.join(self.backup_directory, random)
                 self._download(task, temp_local_filepath)
 
                 self.parser.schedule(ParserPayload("do", temp_local_filepath, task.namespace))
         except BaseException as e:
             self.parser.finish(graceful=False)
             if task is not None:
-                raise DownloadException(task, e)
+                raise DownloadException(task, e) from None
             else:
                 raise
         else:
             self.parser.finish(graceful=True)
         finally:
             self.elapsed = time.time() - start
             self.connection_pool.close()
@@ -626,15 +626,16 @@
             exc: Optional[BaseException] = None
             for downloader_async in downloaders_async:
                 try:
                     downloader_async.result()
                 except BaseException as e:
                     logger.verbose(e)
                     if isinstance(e, DownloadException):
-                        logger.error(f"Failed to download resources {','.join(e.task.resources)} for namespace {e.task.namespace}")
+                        logger.error(f"Failed to download resources {','.join(e.task.resources)} "
+                                     f"for namespace {e.task.namespace}")
                         exc = e.reason
                     else:
                         exc = e
 
             return exc
 
         try:
@@ -688,15 +689,15 @@
 
     cluster.log.verbose('Cleaning up...')
     shutil.rmtree(backup_directory, ignore_errors=True)
 
 
 def pack_to_tgz(target_archive: str, source_dir: str) -> None:
     with tarfile.open(target_archive, "w:gz") as tar_handle:
-        for root, dirs, files in os.walk(source_dir):
+        for root, _, files in os.walk(source_dir):
             for file in files:
                 pathname = os.path.join(root, file)
                 tar_handle.add(pathname, pathname.replace(source_dir, ''))
         tar_handle.close()
 
 
 tasks = OrderedDict({
```

### Comparing `kubemarine-0.28.1/kubemarine/procedures/cert_renew.py` & `kubemarine-0.29.0/kubemarine/procedures/cert_renew.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/procedures/check_iaas.py` & `kubemarine-0.29.0/kubemarine/procedures/check_iaas.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,21 +41,22 @@
 
 
 def connection_ssh_connectivity(cluster: KubernetesCluster) -> None:
     with TestCase(cluster, '001', 'SSH', 'Connectivity', default_results='Connected'):
         try:
             cluster.check_nodes_accessibility(skip_check_iaas=False)
         except KME0006 as e:
-            raise TestFailure(e.summary, hint=e.details)
+            raise TestFailure(e.summary, hint=e.details) from None
 
 
 def connection_ssh_latency_single(cluster: KubernetesCluster) -> None:
+    latency_cfg = static.GLOBALS['compatibility_map']['network']['connection']['latency']['single']
     with TestCase(cluster, '002',  'SSH', 'Latency - Single Thread',
-                  minimal=cluster.globals['compatibility_map']['network']['connection']['latency']['single']['critical'],
-                  recommended=cluster.globals['compatibility_map']['network']['connection']['latency']['single']['recommended']) as tc:
+                  minimal=latency_cfg['critical'],
+                  recommended=latency_cfg['recommended']) as tc:
         i = 0
         measurements = []
         accessible_nodes = cluster.nodes['all'].get_accessible_nodes()
         if accessible_nodes.is_empty():
             return tc.success(results="Skipped")
 
         while i < 5:
@@ -64,30 +65,31 @@
                 time_start = time.time()
                 node.run("echo 1")
                 time_end = time.time()
                 diff = (time_end - time_start) * 1000
                 cluster.log.debug('Connection to %s - %sms' % (node.get_node_name(), diff))
                 measurements.append(diff)
         average_latency = math.floor(sum(measurements) / accessible_nodes.nodes_amount() / 5)
-        if average_latency > cluster.globals['compatibility_map']['network']['connection']['latency']['single']['critical']:
+        if average_latency > latency_cfg['critical']:
             raise TestFailure("Very high latency: %sms" % average_latency,
                               hint="A very high latency was detected between the deploy node and cluster nodes. "
                                    "Check your network settings and status. It is necessary to reduce the latency to %sms."
-                                   % cluster.globals['compatibility_map']['network']['connection']['latency']['single']['critical'])
-        if average_latency > cluster.globals['compatibility_map']['network']['connection']['latency']['single']['recommended']:
+                                   % latency_cfg['critical'])
+        if average_latency > latency_cfg['recommended']:
             raise TestWarn("High latency: %sms" % average_latency,
                            hint="The detected latency is higher than the recommended value (%sms). Check your network settings "
-                                "and status." % cluster.globals['compatibility_map']['network']['connection']['latency']['single']['recommended'])
+                                "and status." % latency_cfg['recommended'])
         tc.success(results="%sms" % average_latency)
 
 
 def connection_ssh_latency_multiple(cluster: KubernetesCluster) -> None:
+    latency_cfg = static.GLOBALS['compatibility_map']['network']['connection']['latency']['multi']
     with TestCase(cluster, '003',  'SSH', 'Latency - Multi Thread',
-                  minimal=cluster.globals['compatibility_map']['network']['connection']['latency']['multi']['critical'],
-                  recommended=cluster.globals['compatibility_map']['network']['connection']['latency']['multi']['recommended']) as tc:
+                  minimal=latency_cfg['critical'],
+                  recommended=latency_cfg['recommended']) as tc:
         i = 0
         measurements = []
         accessible_nodes = cluster.nodes['all'].get_accessible_nodes()
         if accessible_nodes.is_empty():
             return tc.success(results="Skipped")
 
         while i < 10:
@@ -95,23 +97,23 @@
             time_start = time.time()
             accessible_nodes.run("echo 1")
             time_end = time.time()
             diff = (time_end - time_start) * 1000
             cluster.log.debug('Average latency at step %s - %sms' % (i, diff))
             measurements.append(diff)
         average_latency = math.floor(sum(measurements) / 10)
-        if average_latency > cluster.globals['compatibility_map']['network']['connection']['latency']['multi']['critical']:
+        if average_latency > latency_cfg['critical']:
             raise TestFailure("Very high latency: %sms" % average_latency,
                               hint="A very high latency was detected between the deploy node and cluster nodes. "
                                    "Check your network settings and status. It is necessary to reduce the latency to %sms."
-                                   % cluster.globals['compatibility_map']['network']['connection']['latency']['multi']['critical'])
-        if average_latency > cluster.globals['compatibility_map']['network']['connection']['latency']['multi']['recommended']:
+                                   % latency_cfg['critical'])
+        if average_latency > latency_cfg['recommended']:
             raise TestWarn("High latency: %sms" % average_latency,
                            hint="The detected latency is higher than the recommended value (%sms). Check your network settings "
-                                "and status." % cluster.globals['compatibility_map']['network']['connection']['latency']['multi']['recommended'])
+                                "and status." % latency_cfg['recommended'])
         tc.success(results="%sms" % average_latency)
 
 
 def connection_sudoer_access(cluster: KubernetesCluster) -> None:
     with TestCase(cluster, '004', 'SSH', 'Sudoer Access', default_results='Access provided'):
         non_root = []
         for host, node_context in cluster.nodes_context.items():
@@ -129,119 +131,128 @@
 def hardware_members_amount(cluster: KubernetesCluster, group_name: str) -> None:
     beauty_name = group_name.capitalize()
     if group_name == 'vip':
         beauty_name = 'VIP'
     if group_name == 'all':
         beauty_name = 'Total Node'
 
+    hardware_minimal = static.GLOBALS['compatibility_map']['hardware']['minimal'][group_name]
+    hardware_recommended = static.GLOBALS['compatibility_map']['hardware']['recommended'][group_name]
+
     with TestCase(cluster, '005',  'Hardware', '%ss Amount' % beauty_name,
-                  minimal=cluster.globals['compatibility_map']['hardware']['minimal'][group_name]['amount'],
-                  recommended=cluster.globals['compatibility_map']['hardware']['recommended'][group_name]['amount']) as tc:
+                  minimal=hardware_minimal['amount'],
+                  recommended=hardware_recommended['amount']) as tc:
         amount = 0
         if group_name == 'vip':
             amount = len(cluster.inventory.get('vrrp_ips', []))
         else:
             group = cluster.nodes.get(group_name)
             if group is not None:
                 amount = group.nodes_amount()
 
         s = ''
         if amount != 1:
             s = 's'
 
-        if amount < cluster.globals['compatibility_map']['hardware']['minimal'][group_name]['amount']:
+        if amount < hardware_minimal['amount']:
             beauty_name = group_name
             if group_name == 'all':
                 beauty_name = 'all node'
             raise TestFailure("Less than minimal. Detected %s item%s" % (amount, s),
                               hint="Increase the number of resources, so that the number of %ss in the cluster should not "
-                                   "be less than %s." % (beauty_name, cluster.globals['compatibility_map']['hardware']['minimal'][group_name]['amount']))
+                                   "be less than %s." % (beauty_name, hardware_minimal['amount']))
 
-        if amount < cluster.globals['compatibility_map']['hardware']['recommended'][group_name]['amount']:
+        if amount < hardware_recommended['amount']:
             beauty_name = group_name
             if group_name == 'all':
                 beauty_name = 'all node'
             raise TestWarn("Less than recommended. Detected %s item%s" % (amount, s),
                            hint="Increase the number of resources, so that the number of %ss in the cluster should not "
-                                "be less than %s." % (beauty_name, cluster.globals['compatibility_map']['hardware']['minimal'][group_name]['amount']))
+                                "be less than %s." % (beauty_name, hardware_minimal['amount']))
 
         tc.success("%s item%s" % (amount, s))
 
 
 def hardware_cpu(cluster: KubernetesCluster, group_name: str) -> None:
-    minimal_cpu = cluster.globals['compatibility_map']['hardware']['minimal'][group_name]['vcpu'] \
+    hardware_minimal = static.GLOBALS['compatibility_map']['hardware']['minimal'][group_name]
+    hardware_recommended = static.GLOBALS['compatibility_map']['hardware']['recommended'][group_name]
+
+    minimal_cpu = hardware_minimal['vcpu'] \
         if group_name == 'balancer' or cluster.nodes['all'].nodes_amount() > 1 \
-        else cluster.globals['compatibility_map']['hardware']['minimal']['control-plane']['vcpu']
+        else static.GLOBALS['compatibility_map']['hardware']['minimal']['control-plane']['vcpu']
     with TestCase(cluster, '006',  'Hardware', 'VCPUs Amount - %ss' % group_name.capitalize(),
                   minimal=minimal_cpu,
-                  recommended=cluster.globals['compatibility_map']['hardware']['recommended'][group_name]['vcpu']) as tc:
+                  recommended=hardware_recommended['vcpu']) as tc:
         sudo_nodes = cluster.make_group_from_roles([group_name]).get_sudo_nodes()
         if sudo_nodes.is_empty():
             return tc.success(results='Skipped')
         results = sudo_nodes.sudo("nproc --all")
         cluster.log.verbose(results)
         minimal_amount: Optional[int] = None
         for host, result in results.items():
             amount = int(result.stdout)
             if minimal_amount is None or minimal_amount > amount:
                 minimal_amount = amount
             if amount < minimal_cpu:
                 cluster.log.error('%s node %s has insufficient VCPUs: expected %s, but %s found.'
-                                  % (group_name.capitalize(), host, cluster.globals['compatibility_map']['hardware']['minimal'][group_name]['vcpu'], amount))
-            elif amount < cluster.globals['compatibility_map']['hardware']['recommended'][group_name]['vcpu']:
+                                  % (group_name.capitalize(), host, hardware_minimal['vcpu'], amount))
+            elif amount < hardware_recommended['vcpu']:
                 cluster.log.warning('%s node %s has less VCPUs than recommended: recommended %s, but %s found.'
-                                    % (group_name.capitalize(), host, cluster.globals['compatibility_map']['hardware']['recommended'][group_name]['vcpu'], amount))
+                                    % (group_name.capitalize(), host, hardware_recommended['vcpu'], amount))
             else:
                 cluster.log.debug('%s node %s has enough VCPUs: %s' % (group_name.capitalize(), host, amount))
 
         s = ''
         if minimal_amount != 1:
             s = 's'
 
         if minimal_amount < minimal_cpu:
             raise TestFailure("Less than minimal. Detected %s VCPU%s" % (minimal_amount, s),
                               hint="Increase the number of VCPUs in the node configuration to at least the minimum "
-                                   "value: %s VCPUs." % cluster.globals['compatibility_map']['hardware']['minimal'][group_name]['vcpu'])
-        if minimal_amount < cluster.globals['compatibility_map']['hardware']['recommended'][group_name]['vcpu']:
+                                   "value: %s VCPUs." % hardware_minimal['vcpu'])
+        if minimal_amount < hardware_recommended['vcpu']:
             raise TestWarn("Less than recommended. Detected %s VCPU%s" % (minimal_amount, s),
                            hint="Increase the number of VCPUs in the node configuration up to %s VCPUs."
-                                % cluster.globals['compatibility_map']['hardware']['recommended'][group_name]['vcpu'])
+                                % hardware_recommended['vcpu'])
         tc.success(results='%s VCPU%s' % (minimal_amount, s))
 
 
 def hardware_ram(cluster: KubernetesCluster, group_name: str) -> None:
+    hardware_minimal = static.GLOBALS['compatibility_map']['hardware']['minimal'][group_name]
+    hardware_recommended = static.GLOBALS['compatibility_map']['hardware']['recommended'][group_name]
+
     with TestCase(cluster, '007',  'Hardware', 'RAM Amount - %ss' % group_name.capitalize(),
-                  minimal=cluster.globals['compatibility_map']['hardware']['minimal'][group_name]['ram'],
-                  recommended=cluster.globals['compatibility_map']['hardware']['recommended'][group_name]['ram']) as tc:
+                  minimal=hardware_minimal['ram'],
+                  recommended=hardware_recommended['ram']) as tc:
         sudo_nodes = cluster.make_group_from_roles([group_name]).get_sudo_nodes()
         if sudo_nodes.is_empty():
             return tc.success(results='Skipped')
         results = sudo_nodes.sudo("cat /proc/meminfo | awk '/DirectMap/ { print $2 }'")
         cluster.log.verbose(results)
         minimal_amount: Optional[int] = None
         for host, result in results.items():
-            amount = math.floor(sum(map(lambda x: int(x), result.stdout.strip().split("\n"))) / 1000000)
+            amount = math.floor(sum(map(int, result.stdout.strip().split("\n"))) / 1000000)
             if minimal_amount is None or minimal_amount > amount:
                 minimal_amount = amount
-            if amount < cluster.globals['compatibility_map']['hardware']['minimal'][group_name]['ram']:
+            if amount < hardware_minimal['ram']:
                 cluster.log.error('%s node %s has insufficient RAM: expected %sGB, but %sGB found.'
-                                  % (group_name.capitalize(), host, cluster.globals['compatibility_map']['hardware']['minimal'][group_name]['ram'], amount))
-            elif amount < cluster.globals['compatibility_map']['hardware']['recommended'][group_name]['ram']:
+                                  % (group_name.capitalize(), host, hardware_minimal['ram'], amount))
+            elif amount < hardware_recommended['ram']:
                 cluster.log.warning('%s node %s has less RAM than recommended: recommended %sGB, but %sGB found.'
-                                    % (group_name.capitalize(), host, cluster.globals['compatibility_map']['hardware']['recommended'][group_name]['ram'], amount))
+                                    % (group_name.capitalize(), host, hardware_recommended['ram'], amount))
             else:
                 cluster.log.debug('%s node %s has enough RAM: %sGB' % (group_name.capitalize(), host, amount))
-        if minimal_amount < cluster.globals['compatibility_map']['hardware']['minimal'][group_name]['ram']:
+        if minimal_amount < hardware_minimal['ram']:
             raise TestFailure("Less than minimal. Detected %sGB" % minimal_amount,
                               hint="Increase the number of RAM in the node configuration to at least the minimum "
-                                   "value: %sGB." % cluster.globals['compatibility_map']['hardware']['minimal'][group_name]['ram'])
-        if minimal_amount < cluster.globals['compatibility_map']['hardware']['recommended'][group_name]['ram']:
+                                   "value: %sGB." % hardware_minimal['ram'])
+        if minimal_amount < hardware_recommended['ram']:
             raise TestWarn("Less than recommended. Detected %sGB" % minimal_amount,
                            hint="Increase the number of RAM in the node configuration up to %s GB."
-                                % cluster.globals['compatibility_map']['hardware']['recommended'][group_name]['ram'])
+                                % hardware_recommended['ram'])
         tc.success(results='%sGB' % minimal_amount)
 
 
 def system_distributive(cluster: KubernetesCluster) -> None:
     with TestCase(cluster, '008', 'System', 'Distributive') as tc:
         supported_distributives = cluster.globals['compatibility_map']['distributives'].keys()
 
@@ -271,15 +282,16 @@
         detected_supported_os = list(set(detected_supported_os))
         detected_unsupported_os = list(set(detected_unsupported_os))
         detected_unsupported_version = list(set(detected_unsupported_version))
         supported_versions = list(set(supported_versions))
 
         if detected_unsupported_os:
             raise TestFailure("Unsupported OS: %s" % ", ".join(detected_unsupported_os),
-                              hint="Reinstall the OS on the host to one of the supported: %s" % ", ".join(supported_distributives))
+                              hint="Reinstall the OS on the host to one of the supported: %s"
+                                   % ", ".join(supported_distributives))
 
         if detected_unsupported_version:
             raise TestFailure("Unsupported version: %s" % ", ".join(detected_unsupported_version),
                               hint="Reinstall the OS on the host to one of the supported versions: %s" % \
                                       ", ".join(supported_versions))
         
         os_ids = cluster.get_os_identifiers()
@@ -298,15 +310,16 @@
 
 def check_kernel_version(cluster: KubernetesCluster) -> None:
     """
     This method compares the linux kernel version with the bad version
     """
     with TestCase(cluster, '015', "Software", "Kernel version") as tc:
         bad_results = {}
-        unstable_kernel_ubuntu: List[str] = cluster.globals['compatibility_map']['distributives']['ubuntu'][0].get('unstable_kernel')
+        unstable_kernel_ubuntu: List[str] = cluster.globals['compatibility_map']['distributives']['ubuntu'][0] \
+            .get('unstable_kernel')
         unstable_kernel_centos: List[str] = []
         group = cluster.nodes['all'].get_accessible_nodes()
         result_group = group.run('uname -r')
         for host, results in result_group.items():
             os_name = cluster.nodes_context[host]['os']['name']
             result = results.stdout.rstrip()
             if os_name == 'ubuntu':
@@ -324,16 +337,35 @@
         else:
             tc.success("All kernel have stable versions")
 
 
 def check_access_to_thirdparties(cluster: KubernetesCluster) -> None:
     with TestCase(cluster, '012', 'Software', 'Thirdparties Availability') as tc:
         detect_preinstalled_python(cluster)
-        broken = []
-        skipped_msgs = nodes_require_python(cluster)
+        check_resolv_conf(cluster)
+        broken: List[str] = []
+        warnings = nodes_require_python(cluster)
+
+        problem_handlers: Dict[str, List[str]] = {}
+
+        def resolve_problem_handler(host: str) -> List[str]:
+            handler = problem_handlers.get(host)
+            if handler is None:
+                resolv_conf_actual = cluster.nodes_context[host]['resolv_conf_is_actual']
+                if not resolv_conf_actual:
+                    warnings.append(f"resolv.conf is not installed for node {host}: "
+                                    f"Thirdparties can be unavailable. You can install resolv.conf using task "
+                                    f"`install --tasks prepare.dns.resolv_conf`")
+                    handler = warnings
+                else:
+                    handler = broken
+
+                problem_handlers[host] = handler
+
+            return handler
 
         # Load script for checking sources
         all_group = get_python_group(cluster, True)
         check_script = utils.read_internal("resources/scripts/check_url_availability.py")
         random_temp_path = utils.get_remote_tmp_path(ext='py')
         all_group.put(io.StringIO(check_script), random_temp_path)
 
@@ -344,26 +376,27 @@
             # Check with script
             common_group = thirdparties.get_install_group(cluster, config).intersection_group(all_group)
             for node in common_group.get_ordered_members_list():
                 host = node.get_host()
                 python_executable = cluster.nodes_context[host]['python']['executable']
                 res = node.run("%s %s %s %s" % (python_executable, random_temp_path, config['source'],
                                                 cluster.inventory['globals']['timeout_download']), warn=True)
+                problem_handler = resolve_problem_handler(host)
                 if res.is_any_failed():
-                    broken.append(f"{host}, {destination}: {res[host].stderr}")
+                    problem_handler.append(f"{host}, {destination}: {res[host].stderr}")
 
         # Remove file
         rm_command = "rm %s" % random_temp_path
         all_group.run(rm_command)
 
         if broken:
             raise TestFailure('Required thirdparties are unavailable', hint=yaml.safe_dump(broken))
-        if skipped_msgs:
+        if warnings:
             raise TestWarn("Can't detect python version for some nodes",
-                           hint='\n'.join(skipped_msgs))
+                           hint='\n'.join(warnings))
         tc.success('All thirdparties are available')
 
 
 def check_resolv_conf(cluster: KubernetesCluster) -> None:
     nodes_context = cluster.nodes_context
     hosts = [host for host, node_context in nodes_context.items() if 'resolv_conf_is_actual' not in node_context]
 
@@ -778,15 +811,16 @@
             for node in exe.group.get_ordered_members_list():
                 host = node.get_host()
                 node.sudo(f"ip a del {host_to_ip[host]}/{prefix} dev {host_to_inf[host]}",
                           warn=True)
 
 
 @contextmanager
-def assign_random_ips(cluster: KubernetesCluster, group: NodeGroup, host_to_inf: Dict[str, str], subnet: str) -> Iterator[Dict[str, str]]:
+def assign_random_ips(cluster: KubernetesCluster, group: NodeGroup, host_to_inf: Dict[str, str], subnet: str) \
+        -> Iterator[Dict[str, str]]:
     cluster.log.debug(f"Assigning random IP addresses from {subnet} to the internal interface...")
 
     inet = ipaddress.ip_network(subnet)
     prefix = inet.prefixlen
     broadcast = int(inet.broadcast_address)
 
     host_to_ip = {}
@@ -1254,15 +1288,15 @@
         if skipped_msgs:
             raise TestWarn("Cannot complete check", hint='\n'.join(skipped_msgs))
 
         tc.success(results='Connected')
 
 
 def ipip_connectivity(cluster: KubernetesCluster) -> None:
-    with TestCase(cluster, '017', 'Network', 'IP in IP Encapsulation', default_results='Connected') as tc,\
+    with TestCase(cluster, '017', 'Network', 'IP in IP Encapsulation', default_results='Connected'), \
             suspend_firewalld(cluster):
 
         skipped_msgs = []
 
         # Check encapsulation for 'Calico' CNI
         if not cluster.inventory['plugins']['calico']['install']:
             skipped_msgs.append("Calico is not set as CNI for the cluster")
@@ -1274,19 +1308,19 @@
             skipped_msgs.append("Too few nodes, check is skipped")
             raise TestWarn("Check cannot be completed", hint='\n'.join(skipped_msgs))
 
         enc_type = cluster.inventory['plugins']['calico']['mode']
         if enc_type == "ipip":
             # Check if IPv6 addresses are used
             connect_to_ip = group.get_ordered_members_configs_list()[0]['internal_address']
-            if type(ipaddress.ip_address(connect_to_ip)) is not ipaddress.IPv4Address:
+            if utils.isipv(connect_to_ip, [6]):
                 skipped_msgs.append("IPv6 is not supported by IP in IP encapsulation")
                 raise TestWarn("Check cannot be completed", hint='\n'.join(skipped_msgs))
             ip = cluster.inventory['services']['kubeadm']['networking']['podSubnet'].split('/')[0]
-            if type(ipaddress.ip_address(ip)) is not ipaddress.IPv4Address:
+            if utils.isipv(ip, [6]):
                 skipped_msgs.append("IPv6 is not supported by IP in IP encapsulation")
                 raise TestWarn("Check cannot be completed", hint='\n'.join(skipped_msgs))
             failed_nodes = check_ipip_tunnel(group)
         else:
             skipped_msgs.append("Encapsulation IPIP is disabled")
             raise TestWarn("Check cannot be completed", hint='\n'.join(skipped_msgs))
 
@@ -1369,15 +1403,15 @@
         with group_to_rollback.new_executor() as exe:
             for node_exe in exe.group.get_ordered_members_list():
                 node_exe.sudo(f"pkill -9 -P $(cat {ipip_check}.pid | xargs | tr ' ' ','); " \
                               f"sudo rm -f {ipip_check} {ipip_check}.pid", warn=True)
 
 
 def fs_mount_options(cluster: KubernetesCluster) -> None:
-    with TestCase(cluster, '018', 'System', 'Filesystem mount options') as tc:
+    with TestCase(cluster, '018', 'System', 'Filesystem mount options'):
 
         failed_nodes: Set[str] = set()
         cri_root = ""
         # Only Kubernetes nodes should be checked
         group = cluster.make_group_from_roles(['control-plane', 'worker']).get_sudo_nodes()
         # Get CRI root
         if cluster.inventory['services']['cri']['containerRuntime'] == "containerd":
@@ -1390,15 +1424,15 @@
         if cluster.inventory['services']['cri']['containerRuntime'] == "docker":
             # Docker root
             if cluster.inventory['services']['cri']['dockerConfig'].get('data-root', ""):
                 cri_root = cluster.inventory['services']['cri']['dockerConfig']['data-root']
             else:
                 cri_root = "/var/lib/docker"
         if not cri_root:
-                raise TestWarn("Check cannot be completed, unknown CRI")
+            raise TestWarn("Check cannot be completed, unknown CRI")
         cluster.log.debug("Mount options check")
         # Check the mount options for filesystem where containerd root is located.
         # If containerd root doesn't exist the script check the parent directory and so forth.
         # At the end of the script 'findmnt' return the filesytem mount point, device,
         # and mount options for nearest parent directory of CRI root.
         # 'findmnt' perform the recursive search of mount point for filesystem
         # from the given path to the root, that's exactly what we need.
@@ -1528,15 +1562,15 @@
     flow_ = flow.ActionsFlow([IaasAction()])
     result = flow_.run_flow(context, print_summary=False)
 
     testsuite: TestSuite = result.context['testsuite']
 
     # Final summary should be printed only to stdout with custom formatting
     # If test results are required for parsing, they can be found in the test results files
-    print(testsuite.get_final_summary())
+    testsuite.print_final_summary()
     testsuite.print_final_status(result.logger)
     make_reports(context, testsuite)
     return testsuite
 
 
 if __name__ == '__main__':
     testsuite = main()
```

### Comparing `kubemarine-0.28.1/kubemarine/procedures/check_paas.py` & `kubemarine-0.29.0/kubemarine/procedures/check_paas.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,24 +9,25 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import io
+import ipaddress
 import sys
 import time
 from collections import OrderedDict
 import re
 from textwrap import dedent
 from typing import List, Dict, Optional, Union
 
 import yaml
 import ruamel.yaml
-import ipaddress
+from deepdiff import DeepDiff  # type: ignore[import-untyped]
 
 from ordered_set import OrderedSet
 
 from kubemarine import (
     packages as pckgs, system, selinux, etcd, thirdparties, apparmor, kubernetes, sysctl, audit,
     plugins, modprobe, admission
 )
@@ -38,26 +39,25 @@
 from kubemarine.procedures import check_iaas
 from kubemarine.core import flow, static, utils
 from kubemarine.testsuite import TestSuite, TestCase, TestFailure, TestWarn
 from kubemarine.kubernetes.daemonset import DaemonSet
 from kubemarine.kubernetes.deployment import Deployment
 from kubemarine.kubernetes.object import KubernetesObject
 from kubemarine.coredns import generate_configmap
-from deepdiff import DeepDiff  # type: ignore[import-untyped]
 
 
 def services_status(cluster: KubernetesCluster, service_type: str) -> None:
     with TestCase(cluster, '201', "Services", "%s Status" % service_type.capitalize(),
                   default_results='active (running)'):
         group = cluster.nodes['all']
         if service_type == 'haproxy':
             group = cluster.make_group_from_roles(['balancer'])
         elif service_type == 'keepalived':
             group = cluster.make_group_from_roles(['keepalived'])
-        elif service_type == 'docker' or service_type == "containerd" or service_type == 'kubelet':
+        elif service_type in ('docker', 'containerd', 'kubelet'):
             group = cluster.make_group_from_roles(['control-plane', 'worker'])
 
         if group.is_empty():
             raise TestWarn("No nodes to check service status",
                            hint="The node group to check the service is empty. Check skipped.")
 
         collector = CollectorCallback(cluster)
@@ -395,15 +395,15 @@
                 # Create tmp dir for loading thirdparty without default sha
                 random_dir = utils.get_remote_tmp_path()
                 final_commands = "rm -r -f %s" % random_dir
                 random_path = "%s%s" % (random_dir, path)
                 cluster.log.verbose('Temporary path: %s' % random_path)
                 remote_commands = "mkdir -p %s" % ('/'.join(random_path.split('/')[:-1]))
                 # Load thirdparty to temporary dir
-                remote_commands += "&& sudo curl -f -g -s --show-error -L %s -o %s" % (config['source'], random_path)
+                remote_commands += "&& sudo curl -k -f -g -s --show-error -L %s -o %s" % (config['source'], random_path)
                 results = first_control_plane.sudo(remote_commands, warn=True)
                 if results.is_any_failed():
                     host = first_control_plane_host
                     msg = f"Can`t download thirdparty {path} on {host} for getting sha: {results[host].stderr}"
                     broken.append(msg)
                     cluster.log.verbose(msg)
                 else:
@@ -464,15 +464,17 @@
 
             successful.append(path)
             # SHA is correct, now check if it is an archive and if it does, then also check SHA for archive content
             if 'unpack' in config:
                 unpack_dir = config['unpack']
                 extension = path.split('.')[-1]
                 if extension == 'zip': 
-                    res = group.sudo(' unzip -qq -l %s | awk \'NF > 3 { print $4 }\' | while read file_name; do '  # for each file in archive
+                    res = group.sudo(
+                                 # for each file in archive
+                                 ' unzip -qq -l %s | awk \'NF > 3 { print $4 }\' | while read file_name; do '
                                  '  echo ${file_name} '  # print   1) filename
                                  '    $(sudo unzip -p %s ${file_name} | openssl sha1 | cut -d\\  -f2) '  # 2) sha archive
                                  '    $(sudo openssl sha1 %s/${file_name} | cut -d\\  -f2); '  # 3) sha unpacked
                                  'done' % (path, path, unpack_dir)) 
                 else :
                     res = group.sudo('tar tf %s | grep -vw "./" | while read file_name; do '  # for each file in archive
                                  '  echo ${file_name} '  # print   1) filename
@@ -597,15 +599,16 @@
                                    "the node.")
 
         tc.success(results="%s" % ', '.join(positive_conditions))
 
 
 def get_not_running_pods(cluster: KubernetesCluster) -> str:
     # Completed pods should be excluded from the list as well
-    get_pods_cmd = 'kubectl get pods -A --field-selector status.phase!=Running | awk \'{ print $1" "$2" "$4 }\' | grep -vw Completed || true'
+    get_pods_cmd = ('kubectl get pods -A --field-selector status.phase!=Running '
+                    '| awk \'{ print $1" "$2" "$4 }\' | grep -vw Completed || true')
     result = cluster.nodes['control-plane'].get_any_member().sudo(get_pods_cmd)
     cluster.log.verbose(result)
     return list(result.values())[0].stdout.strip()
 
 
 def kubernetes_pods_condition(cluster: KubernetesCluster) -> None:
     system_namespaces = ["kube-system", "ingress-nginx", "kube-public", "kubernetes-dashboard", "default",
@@ -653,27 +656,33 @@
         ingress_ip = cluster.inventory['control_plain']['internal']
 
         if not cluster.inventory['plugins']['kubernetes-dashboard']['install']:
             tc.success(results="skipped")
         else:
             # check dashboard service 
             cluster.log.debug('Check kubernetes-dashboard service...')
+            control_plane = cluster.nodes['control-plane'].get_first_member()
             i = 0
             while not test_service_succeeded and i < retries:
                 i += 1
-                results = cluster.nodes['control-plane'].get_first_member().sudo("kubectl get svc -n kubernetes-dashboard kubernetes-dashboard -o=jsonpath=\"{['spec.clusterIP']}\"", warn=True)
-                for control_plane, result in results.items():
+                results = control_plane.sudo(
+                    "kubectl get svc -n kubernetes-dashboard kubernetes-dashboard "
+                    "-o=jsonpath=\"{['spec.clusterIP']}\"", warn=True)
+                for result in results.values():
                     if result.failed:
                         cluster.log.debug(f'Can not get dashboard service IP: {result.stderr} ')
-                        raise TestFailure("not available",hint=f"Please verify the following Kubernetes Dashboard status and fix this issue")
-                found_url = result.stdout
+                        raise TestFailure("not available",
+                                          hint=f"Please verify the following Kubernetes Dashboard status and fix this issue")
+                found_url = results.get_simple_out()
                 if ipaddress.ip_address(found_url).version == 4:
-                    check_url = cluster.nodes['control-plane'].get_first_member().sudo(f'curl -k -I https://{found_url}:443 -s -S  -w "%{{http_code}}"', warn=True)
+                    check_url = control_plane.sudo(
+                        f'curl -k -I https://{found_url}:443 -s -S  -w "%{{http_code}}"', warn=True)
                 else:
-                    check_url = cluster.nodes['control-plane'].get_first_member().sudo(f'curl -g -k -I https://[{found_url}]:443 -s -S -w "%{{http_code}}"', warn=True)
+                    check_url = control_plane.sudo(
+                        f'curl -g -k -I https://[{found_url}]:443 -s -S -w "%{{http_code}}"', warn=True)
                 status = list(check_url.values())[0].stdout
                 lst = status.split('\n')
                 if lst[len(lst)-1] == '200':
                     cluster.log.verbose(status)
                     cluster.log.debug('Dashboard service is OK')
                     test_service_succeeded = True
                 else:
@@ -681,25 +690,32 @@
                     time.sleep(60)
 
             # check dashboard ingress
             cluster.log.debug('Check kubernetes-dashboard ingress...')
             i = 0
             while not test_ingress_succeeded and test_service_succeeded and i < retries:
                 i += 1
-                results = cluster.nodes['control-plane'].get_first_member().sudo("kubectl -n kubernetes-dashboard get ingress kubernetes-dashboard -o=jsonpath=\"{.spec.rules[0].host}\"", warn=True)
-                for control_plane, result in results.items():
+                results = control_plane.sudo(
+                    "kubectl -n kubernetes-dashboard get ingress kubernetes-dashboard "
+                    "-o=jsonpath=\"{.spec.rules[0].host}\"", warn=True)
+                for result in results.values():
                     if result.failed:
                         cluster.log.debug(f'Can not get dashboard ingress hostname: {result.stderr} ')
-                        raise TestFailure("not available",hint=f"Please verify the following Kubernetes Dashboard status and fix this issue")
-                found_url = result.stdout
+                        raise TestFailure("not available",
+                                          hint=f"Please verify the following Kubernetes Dashboard status and fix this issue")
+                found_url = results.get_simple_out()
                 
                 if ipaddress.ip_address(ingress_ip).version == 4:
-                    check_url = cluster.nodes['control-plane'].get_first_member().sudo(f'curl -k -I -L --resolve {found_url}:443:{ingress_ip} https://{found_url} -s -S -w "%{{http_code}}"', warn=True)
+                    check_url = control_plane.sudo(
+                        f'curl -k -I -L --resolve {found_url}:443:{ingress_ip} https://{found_url} '
+                        f'-s -S -w "%{{http_code}}"', warn=True)
                 else:
-                    check_url = cluster.nodes['control-plane'].get_first_member().sudo(f'curl -g -k -I -L --resolve "{found_url}:443:{ingress_ip}" https://{found_url} -s -S -w "%{{http_code}}"', warn=True)
+                    check_url = control_plane.sudo(
+                        f'curl -g -k -I -L --resolve "{found_url}:443:{ingress_ip}" https://{found_url} '
+                        f'-s -S -w "%{{http_code}}"', warn=True)
                 status = list(check_url.values())[0].stdout
                 lst = status.split('\n')
                 if lst[len(lst)-1] == '200':
                     cluster.log.verbose(status)
                     cluster.log.debug('Dashboard ingress is OK')
                     test_ingress_succeeded = True
                 else:
@@ -784,29 +800,29 @@
                         if pid_max != inventory_pid_max:
                             raise TestWarn("The 'kernel.pid_max' value defined in system = %s, "
                                        "but 'kernel.pid_max', which defined in cluster.yaml = %s"
                                        % (pid_max, inventory_pid_max))
                     if pid_max < required_pid_max:
                         nodes_failed_pid_max_check[node_name] = [pid_max, required_pid_max]
                 else:
-                    cluster.log.error("podPidsLimit is set to unlimited in the /var/lib/kubelet/config.yaml for node '%s'" % node_name)
+                    cluster.log.error("podPidsLimit is set to unlimited in the /var/lib/kubelet/config.yaml "
+                                      f"for node '{node_name}'")
                     nodes_failed_pid_max_check[node_name] = [pid_max, -1]
             else:
                 cluster.log.error("No podPidsLimit set in the /var/lib/kubelet/config.yaml for node '%s'" % node_name)
                 nodes_failed_pid_max_check[node_name] = [pid_max, -1]
 
         if nodes_failed_pid_max_check:
             output = "The requirement for the 'pid_max' value is not met for nodes:\n"
-            for node_name in nodes_failed_pid_max_check:
-                if nodes_failed_pid_max_check[node_name][1] == -1:
+            for node_name, pid_max_check in nodes_failed_pid_max_check.items():
+                if pid_max_check[1] == -1:
                     output += ("For node %s podPidsLimit is unlimited" % node_name)
                 else:
                     output += ("For node %s pid_max value = '%s', but it should be >= then '%s'\n"
-                               % (node_name, nodes_failed_pid_max_check[node_name][0],
-                                  nodes_failed_pid_max_check[node_name][1]))
+                               % (node_name, pid_max_check[0], pid_max_check[1]))
             raise TestFailure(output)
         tc.success(results="pid_max correctly installed on all nodes")
 
 
 def verify_selinux_status(cluster: KubernetesCluster) -> None:
     """
     This method is a test, which checks the status of Selinux. It must be `enforcing`. It may be `permissive`, but must
@@ -815,15 +831,15 @@
     :param cluster: KubernetesCluster object
     :return: None
     """
     with TestCase(cluster, '213', "Security", "Selinux security policy") as tc:
         group = cluster.nodes['all'].get_subgroup_with_os(['rhel', 'rhel8', 'rhel9'])
         if group.is_empty():
             return tc.success("No RHEL nodes found")
-        selinux_configured, selinux_result, selinux_parsed_result = \
+        _, selinux_result, selinux_parsed_result = \
             selinux.is_config_valid(group,
                                     state=selinux.get_expected_state(cluster.inventory),
                                     policy=selinux.get_expected_policy(cluster.inventory),
                                     permissive=selinux.get_expected_permissive(cluster.inventory))
         cluster.log.debug(selinux_result)
         enforcing_ips = []
         permissive_ips = []
@@ -873,15 +889,15 @@
     :param cluster: KubernetesCluster object
     :return: None
     """
     with TestCase(cluster, '214', "Security", "Selinux configuration") as tc:
         group = cluster.nodes['all'].get_subgroup_with_os(['rhel', 'rhel8', 'rhel9'])
         if group.is_empty():
             return tc.success("No RHEL nodes found")
-        selinux_configured, selinux_result, selinux_parsed_result = \
+        selinux_configured, selinux_result, _ = \
             selinux.is_config_valid(group,
                                     state=selinux.get_expected_state(cluster.inventory),
                                     policy=selinux.get_expected_policy(cluster.inventory),
                                     permissive=selinux.get_expected_permissive(cluster.inventory))
         cluster.log.debug(selinux_result)
         if selinux_configured:
             tc.success(results='valid')
@@ -1026,15 +1042,15 @@
     with TestCase(cluster, '219', "ETCD", "Health status ETCD") as tc:
         try:
             etcd_health_status = etcd.wait_for_health(cluster, cluster.nodes['control-plane'].get_any_member())
         except Exception as e:
             cluster.log.verbose('Failed to load and parse ETCD status')
             raise TestFailure('invalid',
                               hint=f"ETCD not ready, please check"
-                                   f" because of {e} ")
+                                   f" because of {e} ") from None
         cluster.log.debug(etcd_health_status)
         tc.success(results='healthy')
 
 
 def container_runtime_configuration_check(cluster: KubernetesCluster) -> None:
     cri_impl: str = cluster.inventory['services']['cri']['containerRuntime']
     with TestCase(cluster, '204', "Services", f"{cri_impl.capitalize()} Configuration Check") as tc:
@@ -1220,26 +1236,28 @@
                     entities_to_check['calico-apiserver'] = {"Deployment": {"calico-apiserver": {"version": expected_version}}}
                 if calico.is_typha_enabled(cluster.inventory):
                     entities_to_check["kube-system"]["Deployment"]["calico-typha"] = {"version": expected_version}
 
             if plugin == 'nginx-ingress-controller':
                 entities_to_check['ingress-nginx'] = {"DaemonSet": {"ingress-nginx-controller": {"version": expected_version}}}
             if plugin == 'local-path-provisioner':
-                entities_to_check['local-path-storage'] = {"Deployment": {"local-path-provisioner": {"version": expected_version}}}
+                entities_to_check['local-path-storage'] = {"Deployment": {
+                    "local-path-provisioner": {"version": expected_version}}}
             if plugin == 'kubernetes-dashboard':
                 image = plugin_item['metrics-scraper']['image']
                 image = image.split('@sha256:')[0]
                 expected_metrics_scrapper_version = image.split(':')[-1]
-                entities_to_check['kubernetes-dashboard'] = {"Deployment": {"kubernetes-dashboard": {"version": expected_version},
-                                                                            "dashboard-metrics-scraper": {"version": expected_metrics_scrapper_version}}}
+                entities_to_check['kubernetes-dashboard'] = {"Deployment": {
+                    "kubernetes-dashboard": {"version": expected_version},
+                    "dashboard-metrics-scraper": {"version": expected_metrics_scrapper_version}}}
 
         for namespace, types_dict in entities_to_check.items():
-            for type, services in types_dict.items():
+            for kind, services in types_dict.items():
                 for service_name, properties in services.items():
-                    k8s_object = KubernetesObject(cluster, type, service_name, namespace)
+                    k8s_object = KubernetesObject(cluster, kind, service_name, namespace)
                     k8s_object.reload(control_plane=first_control_plane, suppress_exceptions=True)
                     if not k8s_object.is_reloaded():
                         stderr = str(k8s_object).rstrip('\n')
                         failed_messages.append(f"failed to load {service_name}: {stderr}")
                         continue
 
                     if properties["version"] not in k8s_object.obj["spec"]["template"]["spec"]["containers"][0].get("image", ""):
@@ -1282,31 +1300,32 @@
                     entities_to_check["kube-system"]["Deployment"].append("calico-typha")
 
             if plugin == 'ingress-nginx-controller':
                 entities_to_check['ingress-nginx'] = {"DaemonSet": ["ingress-nginx-controller"]}
             if plugin == 'local-path-provisioner':
                 entities_to_check['local-path-storage'] = {"Deployment": ["local-path-provisioner"]}
             if plugin == 'kubernetes-dashboard':
-                entities_to_check['kubernetes-dashboard'] = {"Deployment": ["kubernetes-dashboard", "dashboard-metrics-scraper"]}
+                entities_to_check['kubernetes-dashboard'] = {"Deployment": [
+                    "kubernetes-dashboard", "dashboard-metrics-scraper"]}
 
         first_control_plane = cluster.nodes['control-plane'].get_first_member()
         not_ready_entities = []
         for namespace, types_dict in entities_to_check.items():
-            for type, services in types_dict.items():
-                if type == 'DaemonSet':
+            for kind, services in types_dict.items():
+                if kind == 'DaemonSet':
                     for service in services:
                         daemon_set = DaemonSet(cluster, name=service, namespace=namespace)
-                        ready = daemon_set.reload(control_plane=first_control_plane, suppress_exceptions=True).is_actual_and_ready()
-                        if not ready:
+                        daemon_set.reload(control_plane=first_control_plane, suppress_exceptions=True)
+                        if not daemon_set.is_actual_and_ready():
                             not_ready_entities.append(service)
-                elif type == 'Deployment':
+                elif kind == 'Deployment':
                     for service in services:
                         deployment = Deployment(cluster, name=service, namespace=namespace)
-                        ready = deployment.reload(control_plane=first_control_plane, suppress_exceptions=True).is_actual_and_ready()
-                        if not ready:
+                        deployment.reload(control_plane=first_control_plane, suppress_exceptions=True)
+                        if not daemon_set.is_actual_and_ready():
                             not_ready_entities.append(service)
         if len(not_ready_entities) == 0:
             tc.success(results='valid')
         else:
             raise TestFailure('invalid', hint=f"{not_ready_entities} pods doesn't ready")
 
 
@@ -1329,16 +1348,16 @@
     for type_, service_name in entities_to_check:
         k8s_object = KubernetesObject(cluster, type_, service_name, 'kube-system')
         k8s_object.reload(control_plane=first_control_plane, suppress_exceptions=True)
         if not k8s_object.is_reloaded():
             stderr = str(k8s_object).rstrip('\n')
             failed_messages.append(f"failed to load {service_name}: {stderr}")
             continue
-        else:
-            actual_env = get_envs(k8s_object.obj)
+
+        actual_env = get_envs(k8s_object.obj)
 
         expected_obj = manifest_.get_obj(f"{type_}_{service_name}", patch=False)
         buf = io.StringIO()
         utils.yaml_structure_preserver().dump(expected_obj, buf)
         expected_obj = yaml.safe_load(buf.getvalue())
         expected_env = get_envs(expected_obj)
 
@@ -1349,15 +1368,16 @@
             failed_messages.append(f"{service_name!r} env configuration is outdated. Check DEBUG logs for details.")
 
     return failed_messages
 
 
 def calico_config_check(cluster: KubernetesCluster) -> None:
     '''
-    This test checks the configuration of the `calico-node` envs, Calico's ConfigMap in case of `ipam`, and also performed `calicoctl ipam check`.
+    This test checks the configuration of the `calico-node` envs,
+    Calico's ConfigMap in case of `ipam`, and also performed `calicoctl ipam check`.
     :param cluster: KubernetesCluster object
     :return: None
     '''
     with TestCase(cluster, '224', "Calico", "configuration check") as tc:
         first_control_plane = cluster.nodes['control-plane'].get_first_member()
         failed_messages = []
         warn_messages = []
@@ -1372,23 +1392,24 @@
             failed_messages.extend(_check_calico_env(cluster, processor.enrich()))
 
         # Check calico ipam config of CNI config
         result = first_control_plane.sudo(f"kubectl get cm calico-config -n kube-system -oyaml")
         calico_config = yaml.safe_load(result.get_simple_out())
         cni_network_config = yaml.safe_load(calico_config["data"]["cni_network_config"])
         ip = cluster.inventory['services']['kubeadm']['networking']['podSubnet'].split('/')[0]
-        if type(ipaddress.ip_address(ip)) is ipaddress.IPv4Address:
+        if utils.isipv(ip, [4]):
             ipam_config = cluster.inventory["plugins"]["calico"]["cni"]["ipam"]["ipv4"]
         else:
             ipam_config = cluster.inventory["plugins"]["calico"]["cni"]["ipam"]["ipv6"]
         ddiff = DeepDiff(ipam_config, cni_network_config["plugins"][0]["ipam"], ignore_order=True)
         if ddiff:
             cluster.log.debug("'cni_network_config.plugins[0].ipam' of calico-config ConfigMap is outdated:")
             utils.print_diff(cluster.log, ddiff)
-            failed_messages.append("'cni_network_config.plugins[0].ipam' of calico-config ConfigMap is outdated. Check DEBUG logs for details.")
+            failed_messages.append("'cni_network_config.plugins[0].ipam' of calico-config ConfigMap is outdated. "
+                                   "Check DEBUG logs for details.")
 
         # Check calicoctl and calico version match, and check ipam problems.
         result = first_control_plane.sudo("calicoctl ipam check | grep 'found .* problems' |  tr -dc '0-9'")
         found_problems = result.get_simple_result()
         if 'Version mismatch' in found_problems.stderr:
             version_mismatch_lines = found_problems.stderr.split('\n')
 
@@ -1502,15 +1523,16 @@
             broken.append(
                 "Check DEBUG logs for details. "
                 "To have the check passed, you may need to run `kubemarine manage_pss` with enabled pod-security, "
                 "or change the inventory file accordingly."
             )
             raise TestFailure('invalid', hint=yaml.safe_dump(broken))
 
-        kube_admission_status = 'PSS is "enabled", default profile is "%s"' % cluster.inventory["rbac"]["pss"]["defaults"]["enforce"]
+        kube_admission_status = ('PSS is "enabled", default profile is "%s"'
+                                 % cluster.inventory["rbac"]["pss"]["defaults"]["enforce"])
         cluster.log.debug(kube_admission_status)
         tc.success(results='enabled')
 
 
 def geo_check(cluster: KubernetesCluster) -> None:
     """
     This test checks connectivity between clusters in geo schemas using paas-geo-monitor service.
@@ -1806,15 +1828,15 @@
     flow_ = flow.ActionsFlow([PaasAction()])
     result = flow_.run_flow(context, print_summary=False)
 
     testsuite: TestSuite = result.context['testsuite']
 
     # Final summary should be printed only to stdout with custom formatting
     # If tests results required for parsing, they can be found in test results files
-    print(testsuite.get_final_summary(show_minimal=False, show_recommended=False))
+    testsuite.print_final_summary(show_minimal=False, show_recommended=False)
     testsuite.print_final_status(result.logger)
     check_iaas.make_reports(context, testsuite)
     return testsuite
 
 
 if __name__ == '__main__':
     testsuite = main()
```

### Comparing `kubemarine-0.28.1/kubemarine/procedures/config.py` & `kubemarine-0.29.0/kubemarine/procedures/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import json
 import sys
 from typing import List
 
 import yaml
 
 from kubemarine import plugins
-from kubemarine.core import static, utils
+from kubemarine.core import static
 
 HELP_DESCRIPTION = """\
 Print the supported k8s versions with the respective configurations of third-parties.
 
 How to use:
 
 """
@@ -47,14 +47,16 @@
                 kubernetes_version.setdefault('thirdparties', {}) \
                     .setdefault(software, {})['version'] = software_version
 
     return {'kubernetes': kubernetes_versions}
 
 
 def print_config(cfg: dict, arguments: dict) -> None:
+    # pylint: disable=bad-builtin
+
     format_ = arguments['output']
     if format_ == 'yaml':
         print(yaml.safe_dump(cfg, sort_keys=False), end='')
     elif format_ == 'json':
         print(json.dumps(cfg, indent=4))
```

### Comparing `kubemarine-0.28.1/kubemarine/procedures/do.py` & `kubemarine-0.29.0/kubemarine/procedures/do.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 import argparse
 import sys
 from typing import List, Dict, Any
 
 from kubemarine.core import flow
 from kubemarine.core.action import Action
-from kubemarine.core.cluster import KubernetesCluster
+from kubemarine.core.cluster import KubernetesCluster, EnrichmentStage
 from kubemarine.core.group import NodeGroup
 from kubemarine.core.resources import DynamicResources
 
 HELP_DESCRIPTION = """
 Script for executing shell command
     
 additional arguments:
@@ -35,24 +35,24 @@
 class CLIAction(Action):
     def __init__(self, context: dict) -> None:
         super().__init__('do')
         self.do_args: Dict[str, Any] = context['do_arguments']
         self.remote_args: List[str] = context['remote_arguments']
 
     def run(self, res: DynamicResources) -> None:
-        cluster = res.cluster()
+        cluster = res.cluster(EnrichmentStage.LIGHT)
         executors_group = get_executors_group(cluster, self.do_args)
         if executors_group.is_empty():
-            print('Failed to find any of specified nodes or groups')
+            print('Failed to find any of specified nodes or groups')  # pylint: disable=bad-builtin
             sys.exit(1)
 
         no_stream: bool = self.do_args['no_stream']
         result = executors_group.sudo(" ".join(self.remote_args), hide=no_stream, warn=True)
         if no_stream:
-            print(result)
+            print(result)  # pylint: disable=bad-builtin
 
         if result.is_any_failed():
             sys.exit(1)
 
 
 def create_context(cli_arguments: List[str] = None) -> dict:
     if cli_arguments is None:
@@ -93,37 +93,38 @@
         'disable_dump_cleanup': True,
         'log': [
             ['stdout;level=error;colorize=true;correct_newlines=true']
         ],
         'config': configfile_path,
     }, procedure='do')
     context['preserve_inventory'] = False
+    context['make_finalized_inventory'] = False
     context['load_inventory_silent'] = True
 
     context['do_arguments'] = arguments
     context['remote_arguments'] = remote_args
 
     return context
 
 
 def get_executors_group(cluster: KubernetesCluster, arguments: dict) -> NodeGroup:
     if arguments.get('node', None) is not None or arguments.get('group', None) is not None:
-        executor_lists: Dict[str, List[str]] = {
+        executors: Dict[str, List[str]] = {
             'node': [],
             'group': []
         }
-        for executors_type in executor_lists.keys():
+        for executors_type, executor_lists in executors.items():
             executors_str = arguments.get(executors_type)
             if executors_str:
                 if "," in executors_str:
                     for executor_name in executors_str.split(','):
-                        executor_lists[executors_type].append(executor_name.strip())
+                        executor_lists.append(executor_name.strip())
                 else:
-                    executor_lists[executors_type].append(executors_str.strip())
-        return cluster.create_group_from_groups_nodes_names(executor_lists['group'], executor_lists['node'])
+                    executor_lists.append(executors_str.strip())
+        return cluster.create_group_from_groups_nodes_names(executors['group'], executors['node'])
     else:
         return cluster.nodes['control-plane'].get_any_member()
 
 
 def main(cli_arguments: List[str] = None) -> None:
     context = create_context(cli_arguments)
     action = CLIAction(context)
```

### Comparing `kubemarine-0.28.1/kubemarine/procedures/install.py` & `kubemarine-0.29.0/kubemarine/procedures/install.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,16 +62,19 @@
 
         return cluster_wrapper
 
     return roles_wrapper
 
 
 def system_prepare_check_sudoer(cluster: KubernetesCluster) -> None:
+    group = cluster.make_group_from_roles(['control-plane', 'balancer']).include_group(cluster.get_new_nodes_or_self())
     not_sudoers = []
     for host, node_context in cluster.nodes_context.items():
+        if host not in group.nodes:
+            continue
         access_info = node_context['access']
         if access_info['online'] and access_info['sudo'] == 'Root':
             cluster.log.debug("%s online and has root" % host)
         else:
             not_sudoers.append(host)
 
     if not_sudoers:
@@ -214,14 +217,18 @@
         return
 
     system.update_resolv_conf(group, config=cluster.inventory["services"].get("resolv.conf"))
     cluster.log.debug(group.sudo("ls -la /etc/resolv.conf; sudo lsattr /etc/resolv.conf"))
 
 
 def system_prepare_dns_etc_hosts(cluster: KubernetesCluster) -> None:
+    remained_offline = cluster.nodes['all'].get_online_nodes(False)
+    if not remained_offline.is_empty():
+        raise Exception("Nodes %s are not reachable" % remained_offline.get_hosts())
+
     config = system.generate_etc_hosts_config(cluster.inventory, 'etc_hosts')
     config += system.generate_etc_hosts_config(cluster.inventory, 'etc_hosts_generated')
 
     utils.dump_file(cluster, config, 'etc_hosts')
     cluster.log.debug("\nUploading...")
 
     group = cluster.nodes['all']
```

### Comparing `kubemarine-0.28.1/kubemarine/procedures/manage_psp.py` & `kubemarine-0.29.0/kubemarine/procedures/manage_psp.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/procedures/manage_pss.py` & `kubemarine-0.29.0/kubemarine/procedures/manage_pss.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/procedures/migrate_cri.py` & `kubemarine-0.29.0/kubemarine/procedures/migrate_cri.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,14 @@
             control_plane = node
         else:
             control_plane = cluster.nodes["control-plane"].get_first_member()
 
         cluster.log.debug(f'Updating thirdparties for node "{node_name}"...')
         thirdparties.install_all_thirparties(node)
 
-        version = cluster.inventory["services"]["kubeadm"]["kubernetesVersion"]
         cluster.log.debug("Migrating \"%s\"..." % node_name)
         drain_cmd = kubernetes.prepare_drain_command(cluster, node_name, disable_eviction=True)
         control_plane.sudo(drain_cmd, hide=False)
 
         kubeadm_flags_file = "/var/lib/kubelet/kubeadm-flags.env"
         kubeadm_flags = node.sudo(f"cat {kubeadm_flags_file}").get_simple_out()
 
@@ -131,23 +130,26 @@
 
         # delete docker socket
         node.sudo("rm -rf /var/run/docker.sock", hide=False)
 
 
 def release_calico_leaked_ips(cluster: KubernetesCluster) -> None:
     """
-    During drain command we ignore daemon sets, as result this such pods as ingress-nginx-controller arent't deleted before migration.
-    For this reason their ips can stay in calico ipam despite they aren't used. You can check this, if you run "calicoctl ipam check --show-problem-ips" right after apply_new_cri task.
+    During drain command we ignore daemon sets,
+    as result this such pods as ingress-nginx-controller arent't deleted before migration.
+    For this reason their ips can stay in calico ipam despite they aren't used.
+    You can check this, if you run "calicoctl ipam check --show-problem-ips" right after apply_new_cri task.
     Those ips are cleaned by calico garbage collector, but it can take about 20 minutes.
     This task releases problem ips with force.
     """
     first_control_plane = cluster.nodes['control-plane'].get_first_member()
     cluster.log.debug("Getting leaked ips...")
     random_report_name = utils.get_remote_tmp_path(ext='json')
-    result = first_control_plane.sudo(f"calicoctl ipam check --show-problem-ips -o {random_report_name} | grep 'leaked' || true", hide=False)
+    result = first_control_plane.sudo(
+        f"calicoctl ipam check --show-problem-ips -o {random_report_name} | grep 'leaked' || true", hide=False)
     leaked_ips = result.get_simple_out()
     leaked_ips_count = leaked_ips.count('leaked')
     cluster.log.debug(f"Found {leaked_ips_count} leaked ips")
     if leaked_ips_count != 0:
         first_control_plane.sudo(f"calicoctl ipam release --from-report={random_report_name} --force", hide=False)
         cluster.log.debug("Leaked ips was released")
     first_control_plane.sudo(f"rm {random_report_name}", hide=False)
```

### Comparing `kubemarine-0.28.1/kubemarine/procedures/migrate_kubemarine.py` & `kubemarine-0.29.0/kubemarine/procedures/migrate_kubemarine.py`

 * *Files 1% similar despite different names*

```diff
@@ -373,15 +373,16 @@
     def description(self) -> str:
         versions_list = '\n'.join(f" - {ver}" for ver in self.k8s_versions)
 
         return dedent(
             f"""\
             Upgrade {self.plugin_name!r} for the following Kubernetes versions:
             {{versions_list}}
-            Roughly equivalent to 'kubemarine install --tasks=deploy.plugins' with all plugins disabled except the {self.plugin_name!r}.
+            Roughly equivalent to 'kubemarine install --tasks=deploy.plugins'
+            with all plugins disabled except the {self.plugin_name!r}.
             """.rstrip()
         ).format(versions_list=versions_list)
 
 
 def load_upgrade_config() -> dict:
     with utils.open_internal(SOFTWARE_UPGRADE_PATH) as stream:
         upgrade_config: dict = yaml.safe_load(stream)
@@ -471,14 +472,16 @@
     parser.add_argument('procedure_config', metavar='procedure_config',
                         type=str, help='config file for the procedure', nargs='?')
 
     return parser
 
 
 def run(context: dict) -> None:
+    # pylint: disable=bad-builtin
+
     args = context['execution_arguments']
 
     patches = load_patches()
     patch_ids = [patch.identifier for patch in patches]
 
     if args['list']:
         if patch_ids:
```

### Comparing `kubemarine-0.28.1/kubemarine/procedures/reboot.py` & `kubemarine-0.29.0/kubemarine/procedures/reboot.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/procedures/reconfigure.py` & `kubemarine-0.29.0/kubemarine/procedures/reconfigure.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/procedures/remove_node.py` & `kubemarine-0.29.0/kubemarine/procedures/remove_node.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/procedures/restore.py` & `kubemarine-0.29.0/kubemarine/procedures/restore.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,16 @@
     if re.search(r'^\s*$', content):
         return True
 
     return False
 
 
 def replace_config_from_backup_if_needed(procedure_inventory_filepath: str, config: str) -> None:
+    # pylint: disable=bad-builtin
+
     if missing_or_empty(config):
         print('Config is missing or empty - retrieving config from backup archive...')
         procedure = utils.load_yaml(procedure_inventory_filepath)
         if not procedure:
             procedure = {}
         backup_location = procedure.get("backup_location")
         if not backup_location:
@@ -233,22 +235,26 @@
 
     # After restore check db size equal, cluster health and leader elected
     # Checks should be changed
     cluster_status = etcd.wait_for_health(cluster, cluster.nodes['control-plane'].get_any_member())
 
     # Check DB size is correct
     backup_source = cluster.context['backup_descriptor'].get('etcd', {}).get('source')
-    etcd_statuses_from_descriptor = cluster.context['backup_descriptor'].get('etcd', {}).get('status', {})
-    if backup_source and etcd_statuses_from_descriptor and etcd_statuses_from_descriptor.get(backup_source, {}).get('status', {}).get('dbsize'):
-        expected_dbsize = int(etcd_statuses_from_descriptor.get(backup_source, {}).get('status', {}).get('dbsize'))
+    backup_descriptor_dbsize = None
+    if backup_source:
+        backup_descriptor_dbsize = cluster.context['backup_descriptor'].get('etcd', {}).get('status', {}) \
+            .get(backup_source, {}).get('status', {}).get('dbsize')
+    if backup_descriptor_dbsize:
+        expected_dbsize = int(backup_descriptor_dbsize)
         for item in cluster_status:
             real_dbsize = int(item.get('status', {}).get('dbsize'))
             if not real_dbsize:
                 raise Exception('ETCD member "%s" do not have DB size' % item.get('endpoint'))
-            cluster.log.verbose('Endpoint "%s" DB real size %s, expected size %s' % (item.get('endpoint'), expected_dbsize, real_dbsize))
+            cluster.log.verbose('Endpoint "%s" DB real size %s, expected size %s'
+                                % (item.get('endpoint'), expected_dbsize, real_dbsize))
             # restored db should have equal or greater DB size
             if expected_dbsize > real_dbsize:
                 raise Exception('ETCD member "%s" has invalid DB size' % item.get('endpoint'))
         cluster.log.debug('DB size "%s" is correct' % expected_dbsize)
     else:
         cluster.log.verbose('It is not possible to verify db size - descriptor do not contain such information')
```

### Comparing `kubemarine-0.28.1/kubemarine/procedures/upgrade.py` & `kubemarine-0.29.0/kubemarine/procedures/upgrade.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import itertools
-import os
 from collections import OrderedDict
 from typing import List, Callable, Dict
 
 from kubemarine import kubernetes, plugins, admission, jinja
 from kubemarine.core import flow, log, resources as res
 from kubemarine.core import utils
 from kubemarine.core.cluster import KubernetesCluster, EnrichmentStage
```

### Comparing `kubemarine-0.28.1/kubemarine/resources/__init__.py` & `kubemarine-0.29.0/kubemarine/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/configurations/__init__.py` & `kubemarine-0.29.0/kubemarine/resources/configurations/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/configurations/compatibility/internal/kubernetes_images.yaml` & `kubemarine-0.29.0/kubemarine/resources/configurations/compatibility/internal/kubernetes_images.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,16 @@
     version: v1.28.0
   v1.28.3:
     version: v1.28.3
   v1.28.4:
     version: v1.28.4
   v1.28.6:
     version: v1.28.6
+  v1.28.8:
+    version: v1.28.8
   v1.29.1:
     version: v1.29.1
 kube-controller-manager:
   v1.23.1:
     version: v1.23.1
   v1.23.6:
     version: v1.23.6
@@ -76,14 +78,16 @@
     version: v1.28.0
   v1.28.3:
     version: v1.28.3
   v1.28.4:
     version: v1.28.4
   v1.28.6:
     version: v1.28.6
+  v1.28.8:
+    version: v1.28.8
   v1.29.1:
     version: v1.29.1
 kube-scheduler:
   v1.23.1:
     version: v1.23.1
   v1.23.6:
     version: v1.23.6
@@ -117,14 +121,16 @@
     version: v1.28.0
   v1.28.3:
     version: v1.28.3
   v1.28.4:
     version: v1.28.4
   v1.28.6:
     version: v1.28.6
+  v1.28.8:
+    version: v1.28.8
   v1.29.1:
     version: v1.29.1
 kube-proxy:
   v1.23.1:
     version: v1.23.1
   v1.23.6:
     version: v1.23.6
@@ -158,14 +164,16 @@
     version: v1.28.0
   v1.28.3:
     version: v1.28.3
   v1.28.4:
     version: v1.28.4
   v1.28.6:
     version: v1.28.6
+  v1.28.8:
+    version: v1.28.8
   v1.29.1:
     version: v1.29.1
 pause:
   v1.23.1:
     version: '3.6'
   v1.23.6:
     version: '3.6'
@@ -199,14 +207,16 @@
     version: '3.9'
   v1.28.3:
     version: '3.9'
   v1.28.4:
     version: '3.9'
   v1.28.6:
     version: '3.9'
+  v1.28.8:
+    version: '3.9'
   v1.29.1:
     version: '3.9'
 etcd:
   v1.23.1:
     version: 3.5.1-0
   v1.23.6:
     version: 3.5.1-0
@@ -240,14 +250,16 @@
     version: 3.5.9-0
   v1.28.3:
     version: 3.5.9-0
   v1.28.4:
     version: 3.5.9-0
   v1.28.6:
     version: 3.5.10-0
+  v1.28.8:
+    version: 3.5.12-0
   v1.29.1:
     version: 3.5.10-0
 coredns/coredns:
   v1.23.1:
     version: v1.8.6
   v1.23.6:
     version: v1.8.6
@@ -281,9 +293,11 @@
     version: v1.10.1
   v1.28.3:
     version: v1.10.1
   v1.28.4:
     version: v1.10.1
   v1.28.6:
     version: v1.10.1
+  v1.28.8:
+    version: v1.10.1
   v1.29.1:
     version: v1.11.1
```

### Comparing `kubemarine-0.28.1/kubemarine/resources/configurations/compatibility/internal/packages.yaml` & `kubemarine-0.29.0/kubemarine/resources/configurations/compatibility/internal/packages.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -96,14 +96,19 @@
     version_rhel9: 20.10*
     version_debian: 5:20.10.*
   v1.28.6:
     version_rhel: 19.03*
     version_rhel8: 19.03*
     version_rhel9: 20.10*
     version_debian: 5:20.10.*
+  v1.28.8:
+    version_rhel: 19.03*
+    version_rhel8: 19.03*
+    version_rhel9: 20.10*
+    version_debian: 5:20.10.*
   v1.29.1:
     version_rhel: 19.03*
     version_rhel8: 19.03*
     version_rhel9: 20.10*
     version_debian: 5:20.10.*
 containerd:
   v1.23.1:
@@ -140,14 +145,16 @@
     version_debian: 1.6.*
   v1.28.3:
     version_debian: 1.6.*
   v1.28.4:
     version_debian: 1.6.*
   v1.28.6:
     version_debian: 1.6.*
+  v1.28.8:
+    version_debian: 1.6.*
   v1.29.1:
     version_debian: 1.6.*
 containerdio:
   v1.23.1:
     version_rhel: 1.6*
     version_rhel8: 1.6*
     version_rhel9: 1.6*
@@ -238,14 +245,19 @@
     version_rhel9: 1.6*
     version_debian: 1.6.*
   v1.28.6:
     version_rhel: 1.6*
     version_rhel8: 1.6*
     version_rhel9: 1.6*
     version_debian: 1.6.*
+  v1.28.8:
+    version_rhel: 1.6*
+    version_rhel8: 1.6*
+    version_rhel9: 1.6*
+    version_debian: 1.6.*
   v1.29.1:
     version_rhel: 1.6*
     version_rhel8: 1.6*
     version_rhel9: 1.6*
     version_debian: 1.6.*
 haproxy:
   version_rhel: 1.8*
```

### Comparing `kubemarine-0.28.1/kubemarine/resources/configurations/compatibility/internal/plugins.yaml` & `kubemarine-0.29.0/kubemarine/resources/configurations/compatibility/internal/plugins.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,16 @@
     version: v3.26.4
   v1.28.3:
     version: v3.26.4
   v1.28.4:
     version: v3.26.4
   v1.28.6:
     version: v3.27.0
+  v1.28.8:
+    version: v3.27.0
   v1.29.1:
     version: v3.27.0
 nginx-ingress-controller:
   v1.23.1:
     version: v1.2.0
     webhook-version: v1.1.1
   v1.23.6:
@@ -99,17 +101,20 @@
     webhook-version: v20231011-8b53cabe0
   v1.28.4:
     version: v1.9.4
     webhook-version: v20231011-8b53cabe0
   v1.28.6:
     version: v1.9.5
     webhook-version: v20231011-8b53cabe0
+  v1.28.8:
+    version: v1.9.6
+    webhook-version: v20231226-1a7112e06
   v1.29.1:
-    version: v1.9.5
-    webhook-version: v20231011-8b53cabe0
+    version: v1.9.6
+    webhook-version: v20231226-1a7112e06
 kubernetes-dashboard:
   v1.23.1:
     version: v2.5.1
     metrics-scraper-version: v1.0.7
   v1.23.6:
     version: v2.5.1
     metrics-scraper-version: v1.0.7
@@ -160,14 +165,17 @@
     metrics-scraper-version: v1.0.8
   v1.28.4:
     version: v2.7.0
     metrics-scraper-version: v1.0.8
   v1.28.6:
     version: v2.7.0
     metrics-scraper-version: v1.0.8
+  v1.28.8:
+    version: v2.7.0
+    metrics-scraper-version: v1.0.8
   v1.29.1:
     version: v2.7.0
     metrics-scraper-version: v1.0.8
 local-path-provisioner:
   v1.23.1:
     version: v0.0.22
     busybox-version: 1.34.1
@@ -221,10 +229,13 @@
     busybox-version: 1.34.1
   v1.28.4:
     version: v0.0.25
     busybox-version: 1.34.1
   v1.28.6:
     version: v0.0.26
     busybox-version: 1.34.1
+  v1.28.8:
+    version: v0.0.26
+    busybox-version: 1.34.1
   v1.29.1:
     version: v0.0.26
     busybox-version: 1.34.1
```

### Comparing `kubemarine-0.28.1/kubemarine/resources/configurations/compatibility/internal/thirdparties.yaml` & `kubemarine-0.29.0/kubemarine/resources/configurations/compatibility/internal/thirdparties.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,16 @@
     sha1: e03127bc6605f4518c449e543c142ec69bf37798
   v1.28.3:
     sha1: 8935140d6a7b64f9038c911246cfc2a8da843673
   v1.28.4:
     sha1: 450eef85788fb68c4c26db82c6a0fb222e07869d
   v1.28.6:
     sha1: a6846fe15ce29865e9c813a677f40dc21868223c
+  v1.28.8:
+    sha1: 75f719839be79baa3b66df225af7f1edf1b06501
   v1.29.1:
     sha1: 14390d6df2bb0b6546efd2238068c300461053fd
 kubelet:
   v1.23.1:
     sha1: 4a7e2e5f5e6b8e95efa52931786bc275a037bc50
   v1.23.6:
     sha1: 326110dcb62b66e69490d039b170682fb71c5560
@@ -77,14 +79,16 @@
     sha1: d096ad117047f368a5c4c37d511aacd612691aba
   v1.28.3:
     sha1: de8824a4eac34277251f911e944c69488359ee69
   v1.28.4:
     sha1: 32ef1daaf8f4996d16ff386f44cc0555c6f3de24
   v1.28.6:
     sha1: 25e2675bcbc59004ef148dc91a25404132b1faa1
+  v1.28.8:
+    sha1: 9febc78ac9e887762d2ea74fc58972c7e2354af0
   v1.29.1:
     sha1: aa871f4656bf1cc6393058f28d5c938268df3d4e
 kubectl:
   v1.23.1:
     sha1: 4ceb8d046a2d8253495aa86d13f11e2eb29644fc
   v1.23.6:
     sha1: 65a24196b4cc9a3d2eafbd254b9d2d4add8ba152
@@ -118,14 +122,16 @@
     sha1: c456a5e8541a6c9fbcf199ff65b37559bdd29925
   v1.28.3:
     sha1: 096796f53a9b5af22e9e14b694fdefc870182b6e
   v1.28.4:
     sha1: 9a1691d307cb419d7047baccba89765015b2b7a4
   v1.28.6:
     sha1: 1458cc8aa68c2c4406db9fb36eeff181460d7f65
+  v1.28.8:
+    sha1: be53272620f4d0422cb209d0ebfb248666be837c
   v1.29.1:
     sha1: 5867f210ce90c62e0551062492751e43c2ae6a46
 calicoctl:
 # calicoctl version is duplicated from kubemarine/resources/configurations/compatibility/kubernetes_versions.yaml
 # It also corresponds to the plugin version in kubemarine/resources/configurations/compatibility/internal/plugins.yaml
   v1.23.1:
     version: v3.24.2
@@ -180,14 +186,17 @@
     sha1: 46875b3d28318553fe382db0766a0916f2556217
   v1.28.4:
     version: v3.26.4
     sha1: 46875b3d28318553fe382db0766a0916f2556217
   v1.28.6:
     version: v3.27.0
     sha1: 4d62cba82a4aee97ab20b96e7270da85d77ce20e
+  v1.28.8:
+    version: v3.27.0
+    sha1: 4d62cba82a4aee97ab20b96e7270da85d77ce20e
   v1.29.1:
     version: v3.27.0
     sha1: 4d62cba82a4aee97ab20b96e7270da85d77ce20e
 crictl:
 # crictl version is duplicated from kubemarine/resources/configurations/compatibility/kubernetes_versions.yaml
 # for backward compatibility with clusters in a private environment.
   v1.23.1:
@@ -243,10 +252,13 @@
     sha1: 1199411456ab5a1e0dd9524724f15e92aa3f9da7
   v1.28.4:
     version: v1.28.0
     sha1: 1199411456ab5a1e0dd9524724f15e92aa3f9da7
   v1.28.6:
     version: v1.29.0
     sha1: c4224ed25f729dbf73976198c8bc73dec0bf5a5f
+  v1.28.8:
+    version: v1.29.0
+    sha1: c4224ed25f729dbf73976198c8bc73dec0bf5a5f
   v1.29.1:
     version: v1.29.0
     sha1: c4224ed25f729dbf73976198c8bc73dec0bf5a5f
```

### Comparing `kubemarine-0.28.1/kubemarine/resources/configurations/compatibility/kubernetes_versions.yaml` & `kubemarine-0.29.0/kubemarine/resources/configurations/compatibility/kubernetes_versions.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -127,17 +127,23 @@
     crictl: v1.28.0
   v1.28.6:
     calico: v3.27.0
     nginx-ingress-controller: v1.9.5
     kubernetes-dashboard: v2.7.0
     local-path-provisioner: v0.0.26
     crictl: v1.29.0
+  v1.28.8:
+    calico: v3.27.0
+    nginx-ingress-controller: v1.9.6
+    kubernetes-dashboard: v2.7.0
+    local-path-provisioner: v0.0.26
+    crictl: v1.29.0
   v1.29.1:
     calico: v3.27.0
-    nginx-ingress-controller: v1.9.5
+    nginx-ingress-controller: v1.9.6
     kubernetes-dashboard: v2.7.0
     local-path-provisioner: v0.0.26
     crictl: v1.29.0
 
 # After any change, please run scripts/thirdparties/sync.py
 
 # The following optional keys are supported in addition to the 5 required software keys:
```

### Comparing `kubemarine-0.28.1/kubemarine/resources/configurations/defaults.yaml` & `kubemarine-0.29.0/kubemarine/resources/configurations/defaults.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -12,20 +12,20 @@
       plugins:
         timeout: 5
         retries: 150
   nodes:
     ready:
       timeout: 5
       retries: 15
-    boot:
-     timeout: 600
   timeout_download:
     60
 
-node_defaults: {}
+node_defaults:
+  boot:
+    timeout: 600
 
 nodes: []
 
 public_cluster_ip: '{{ control_plain.external }}'
 
 services:
   kubeadm_kubelet:
@@ -33,14 +33,15 @@
     kind: KubeletConfiguration
     readOnlyPort: 0
     enableDebuggingHandlers: true
     protectKernelDefaults: true
     podPidsLimit: 4096
     cgroupDriver: systemd
     serializeImagePulls: false
+    tlsCipherSuites: [TLS_ECDHE_ECDSA_WITH_AES_128_GCM_SHA256,TLS_ECDHE_RSA_WITH_AES_128_GCM_SHA256,TLS_ECDHE_ECDSA_WITH_CHACHA20_POLY1305,TLS_ECDHE_RSA_WITH_AES_256_GCM_SHA384,TLS_ECDHE_RSA_WITH_CHACHA20_POLY1305,TLS_ECDHE_ECDSA_WITH_AES_256_GCM_SHA384,TLS_RSA_WITH_AES_256_GCM_SHA384,TLS_RSA_WITH_AES_128_GCM_SHA256]
   kubeadm_kube-proxy:
     apiVersion: kubeproxy.config.k8s.io/v1alpha1
     kind: KubeProxyConfiguration
     conntrack: {}
   kubeadm_flags:
     ignorePreflightErrors: Port-6443,CoreDNSUnsupportedPlugins
   kubeadm:
@@ -563,15 +564,15 @@
               manifest_id: apiserver
         - python:
             module: plugins/calico.py
             method: renew_apiserver_certificate
     mode: ipip
     crossSubnet: true
     natOutgoing: true
-    mtu: 1440
+    mtu: 1430
     fullmesh: true
     announceServices: false
     defaultAsNumber: 64512
     globalBgpPeers: []
     typha:
       # enabled by default for envs with nodes > 3
       enabled: '{% if (nodes | select("has_roles", ["control-plane", "worker"]) | list | length) < 4 %}false{% else %}true{% endif %}'
```

### Comparing `kubemarine-0.28.1/kubemarine/resources/configurations/globals.yaml` & `kubemarine-0.29.0/kubemarine/resources/configurations/globals.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -356,14 +356,15 @@
         versions:
           - '8.6'
           - '8.7'
           - '8.8'
       - os_family: 'rhel9'
         versions:
           - '9.2'
+          - '9.3'
     ubuntu:
       - os_family: 'debian'
         versions:
           - '20.04'
           - '22.04'
         unstable_kernel:
           - '5.4.0-132-generic'
```

### Comparing `kubemarine-0.28.1/kubemarine/resources/drop_ins/__init__.py` & `kubemarine-0.29.0/kubemarine/resources/drop_ins/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/etalons/patches/__init__.py` & `kubemarine-0.29.0/kubemarine/patches/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,14 +18,18 @@
 
 The whole directory is automatically cleared and reset after new version of Kubemarine is released.
 """
 
 from typing import List
 
 from kubemarine.core.patch import Patch
+from kubemarine.patches.boot_timeout_per_node import TimeoutPerNode
+from kubemarine.patches.strong_cipher_suits_for_kubelet import UpdatekubeletCipherSuites
 
 patches: List[Patch] = [
+    TimeoutPerNode(),
+    UpdatekubeletCipherSuites(),  # Add the new patch to the list
 ]
 """
 List of patches that is sorted according to the Patch.priority() before execution.
 Patches that have the same priority, are executed in the declared order.
 """
```

### Comparing `kubemarine-0.28.1/kubemarine/resources/etalons/patches/software_upgrade.yaml` & `kubemarine-0.29.0/kubemarine/patches/software_upgrade.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -31,10 +31,11 @@
   keepalived:
     version_rhel: false
     version_rhel8: false
     version_rhel9: false
     version_debian: false
 plugins:
   calico: []
-  nginx-ingress-controller: []
+  nginx-ingress-controller:
+  - v1.29.1
   kubernetes-dashboard: []
   local-path-provisioner: []
```

### Comparing `kubemarine-0.28.1/kubemarine/resources/psp/__init__.py` & `kubemarine-0.29.0/kubemarine/resources/psp/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/psp/anyuid.yaml` & `kubemarine-0.29.0/kubemarine/resources/psp/anyuid.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/psp/default.yaml` & `kubemarine-0.29.0/kubemarine/resources/psp/default.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/psp/host-network.yaml` & `kubemarine-0.29.0/kubemarine/resources/psp/host-network.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/psp/privileged.yaml` & `kubemarine-0.29.0/kubemarine/resources/psp/privileged.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/reports/__init__.py` & `kubemarine-0.29.0/kubemarine/resources/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/reports/check_report.css` & `kubemarine-0.29.0/kubemarine/resources/reports/check_report.css`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/backup.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/backup.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/cert_renew.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/cert_renew.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/cluster.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/cluster.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8277777777777778%*

 * *Differences: {"'definitions'": "OrderedDict([('GatewayNodes', OrderedDict([('type', 'array'), ('description', "*

 * *                  "'Specify the gateway nodes through which you need to create an SSH-tunnel.'), "*

 * *                  "('items', OrderedDict([('$ref', 'definitions/gateway_node.json')]))])), "*

 * *                  "('ProcedureHistory', OrderedDict([('type', 'object'), ('description', "*

 * *                  "'Parameters for the inventory preservation on nodes after each procedure "*

 * *                  "run.'), ('propert […]*

```diff
@@ -1,10 +1,36 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema",
     "additionalProperties": false,
+    "definitions": {
+        "GatewayNodes": {
+            "description": "Specify the gateway nodes through which you need to create an SSH-tunnel.",
+            "items": {
+                "$ref": "definitions/gateway_node.json"
+            },
+            "type": "array"
+        },
+        "ProcedureHistory": {
+            "additionalProperties": false,
+            "description": "Parameters for the inventory preservation on nodes after each procedure run.",
+            "properties": {
+                "archive_threshold": {
+                    "default": 5,
+                    "description": "Number of procedure runs after which the information about old runs is archived.",
+                    "type": "integer"
+                },
+                "delete_threshold": {
+                    "default": 10,
+                    "description": "Number of procedure runs after which the information about old runs is deleted.",
+                    "type": "integer"
+                }
+            },
+            "type": "object"
+        }
+    },
     "properties": {
         "cluster_name": {
             "description": "Address of the cluster. On this address, the Control Plane Endpoint is raised, and it is used in the calculated parameters.",
             "type": "string"
         },
         "control_plain": {
             "additionalProperties": false,
@@ -18,19 +44,15 @@
                     "description": "Internal network address for the connection. It is to be used for all internal kubeapi traffic.",
                     "type": "string"
                 }
             },
             "type": "object"
         },
         "gateway_nodes": {
-            "description": "Specify the gateway nodes through which you need to create an SSH-tunnel.",
-            "items": {
-                "$ref": "definitions/gateway_node.json"
-            },
-            "type": "array"
+            "$ref": "#/definitions/GatewayNodes"
         },
         "globals": {
             "$ref": "definitions/globals.json"
         },
         "node_defaults": {
             "$ref": "definitions/node_defaults.json"
         },
@@ -45,29 +67,15 @@
         "plugin_defaults": {
             "$ref": "definitions/plugin_defaults.json"
         },
         "plugins": {
             "$ref": "definitions/plugins.json"
         },
         "procedure_history": {
-            "additionalProperties": false,
-            "description": "Parameters for the inventory preservation on nodes after each procedure run.",
-            "properties": {
-                "archive_threshold": {
-                    "default": 5,
-                    "description": "Number of procedure runs after which the information about old runs is archived.",
-                    "type": "integer"
-                },
-                "delete_threshold": {
-                    "default": 10,
-                    "description": "Number of procedure runs after which the information about old runs is deleted.",
-                    "type": "integer"
-                }
-            },
-            "type": "object"
+            "$ref": "#/definitions/ProcedureHistory"
         },
         "public_cluster_ip": {
             "default": "'{{ control_plain.external }}'",
             "description": "An obsolete variable that is used if you are using Helm plugins installation.",
             "type": "string"
         },
         "rbac": {
```

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/common/node_ref.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/common/node_ref.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/common/utils.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/common/utils.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/gateway_node.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/gateway_node.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8214285714285714%*

 * *Differences: {"'allOf'": "{insert: [(1, OrderedDict([('$ref', "*

 * *            "'node_defaults.json#/definitions/OneOfKeyfilePasswordSpec')]))]}",*

 * * 'delete': "['oneOf']"}*

```diff
@@ -1,24 +1,15 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema",
     "allOf": [
         {
             "$ref": "node_defaults.json#/definitions/SSHAccessCommonProperties"
-        }
-    ],
-    "oneOf": [
-        {
-            "required": [
-                "keyfile"
-            ]
         },
         {
-            "required": [
-                "password"
-            ]
+            "$ref": "node_defaults.json#/definitions/OneOfKeyfilePasswordSpec"
         }
     ],
     "properties": {
         "address": {
             "description": "Gateway node's IP or hostname address for connection",
             "type": "string"
         },
```

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/globals.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/globals.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9973958333333334%*

 * *Differences: {"'definitions'": "{'Nodes': {'properties': {delete: ['boot']}}}"}*

```diff
@@ -2,27 +2,14 @@
     "$schema": "http://json-schema.org/draft-07/schema",
     "additionalProperties": false,
     "definitions": {
         "Nodes": {
             "additionalProperties": false,
             "description": "Section to hold mostly timeout-related settings, global for nodes",
             "properties": {
-                "boot": {
-                    "additionalProperties": false,
-                    "description": "Nodes boot settings",
-                    "properties": {
-                        "timeout": {
-                            "default": 600,
-                            "description": "Timeout for node reboot in seconds",
-                            "minimal": 1,
-                            "type": "integer"
-                        }
-                    },
-                    "type": "object"
-                },
                 "ready": {
                     "additionalProperties": false,
                     "description": "Settings for Kubernetes nodes readiness check",
                     "properties": {
                         "retries": {
                             "default": 30,
                             "description": "Number of retries for node readiness check",
```

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/node.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/node.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.953125%*

 * *Differences: {"'definitions'": "{'Properties': {'allOf': {0: {'$ref': '#/definitions/AccessProperties'}}, "*

 * *                  "'properties': {delete: ['name', 'address', 'internal_address', 'connect_to']}}, "*

 * *                  "'PropertyNames': {'anyOf': {0: {'$ref': '#/definitions/AccessPropertyNames'}, "*

 * *                  "1: {'enum': {delete: [5, 2, 1, 0]}}}}, 'AccessProperties': "*

 * *                  "OrderedDict([('allOf', [OrderedDict([('$ref', "*

 * *                  "'node_defaults.json#/definitions/CommonNodeProperti […]*

```diff
@@ -2,60 +2,80 @@
     "$schema": "http://json-schema.org/draft-07/schema",
     "allOf": [
         {
             "$ref": "#/definitions/Properties"
         }
     ],
     "definitions": {
-        "Properties": {
+        "AccessProperties": {
             "allOf": [
                 {
                     "$ref": "node_defaults.json#/definitions/CommonNodeProperties"
                 }
             ],
             "properties": {
                 "address": {
                     "description": "External node's IP-address",
                     "type": "string"
                 },
                 "connect_to": {
                     "type": "string"
                 },
-                "control_endpoint": {
-                    "default": false,
-                    "description": "Parameter to help the algorithm in choosing which address to take as the control_plain",
-                    "type": "boolean"
-                },
                 "internal_address": {
                     "description": "Internal node's IP-address",
                     "type": "string"
                 },
                 "name": {
                     "$ref": "common/node_ref.json#/definitions/Name",
                     "description": "Cluster member name. If omitted, KubeMarine will calculate the name by the member role and position in the inventory."
+                }
+            }
+        },
+        "AccessPropertyNames": {
+            "anyOf": [
+                {
+                    "$ref": "node_defaults.json#/definitions/CommonNodePropertyNames"
+                },
+                {
+                    "enum": [
+                        "name",
+                        "address",
+                        "internal_address",
+                        "connect_to"
+                    ]
+                }
+            ]
+        },
+        "Properties": {
+            "allOf": [
+                {
+                    "$ref": "#/definitions/AccessProperties"
+                }
+            ],
+            "properties": {
+                "control_endpoint": {
+                    "default": false,
+                    "description": "Parameter to help the algorithm in choosing which address to take as the control_plain",
+                    "type": "boolean"
                 },
                 "roles": {
                     "$ref": "common/node_ref.json#/definitions/Roles",
                     "description": "Cluster member roles"
                 }
             }
         },
         "PropertyNames": {
             "anyOf": [
                 {
-                    "$ref": "node_defaults.json#/definitions/CommonNodePropertyNames"
+                    "$ref": "#/definitions/AccessPropertyNames"
                 },
                 {
                     "enum": [
-                        "name",
-                        "address",
-                        "internal_address",
                         "roles",
-                        "control_endpoint",
-                        "connect_to"
+                        "control_endpoint"
                     ]
                 }
             ]
         }
     },
     "propertyNames": {
         "$ref": "#/definitions/PropertyNames"
```

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/node_defaults.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/installation/expect.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.3333333333333333%*

 * *Differences: {"'additionalProperties'": 'False',*

 * * "'definitions'": "{replace: OrderedDict([('GenericResource', OrderedDict([('description', 'Type "*

 * *                  'of Kubernetes resources. Can be either a list of names or a dictionary with the '*

 * *                  "extra parameters.'), ('oneOf', [OrderedDict([('$ref', "*

 * *                  "'#/definitions/ResourcesList')]), OrderedDict([('type', 'object'), ('allOf', "*

 * *                  "[OrderedDict([('$ref', '#/definitions/CommonResourceProperties')])]), "*

 * *             […]*

```diff
@@ -1,96 +1,150 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema",
-    "allOf": [
-        {
-            "$ref": "#/definitions/CommonNodeProperties"
-        }
-    ],
+    "additionalProperties": false,
     "definitions": {
-        "CommonNodeProperties": {
-            "allOf": [
-                {
-                    "$ref": "#/definitions/SSHAccessCommonProperties"
-                }
-            ],
+        "CommonResourceProperties": {
             "properties": {
-                "gateway": {
-                    "description": "Gateway that should be used to connect to node(s)",
-                    "type": "string"
-                },
-                "labels": {
-                    "additionalProperties": {
-                        "type": [
-                            "string",
-                            "boolean",
-                            "integer"
-                        ]
-                    },
-                    "description": "Additional labels for node(s)",
-                    "type": "object"
+                "retries": {
+                    "default": 30,
+                    "description": "The number of attempts to check the status",
+                    "type": "integer"
                 },
-                "taints": {
-                    "$ref": "common/utils.json#/definitions/ArrayOfStrings",
-                    "description": "Additional taints for node(s). Caution: Use at your own risk. It can cause unexpected behavior. No support is provided for consequences."
+                "timeout": {
+                    "default": 5,
+                    "description": "The number of seconds until the next resource status check",
+                    "type": "integer"
                 }
             }
         },
-        "CommonNodePropertyNames": {
-            "anyOf": [
+        "CommonResourcePropertyNames": {
+            "enum": [
+                "timeout",
+                "retries"
+            ]
+        },
+        "GenericResource": {
+            "description": "Type of Kubernetes resources. Can be either a list of names or a dictionary with the extra parameters.",
+            "oneOf": [
                 {
-                    "$ref": "#/definitions/SSHAccessCommonPropertyNames"
+                    "$ref": "#/definitions/ResourcesList"
                 },
                 {
-                    "enum": [
-                        "labels",
-                        "taints",
-                        "gateway"
-                    ]
+                    "allOf": [
+                        {
+                            "$ref": "#/definitions/CommonResourceProperties"
+                        }
+                    ],
+                    "properties": {
+                        "list": {
+                            "$ref": "#/definitions/ResourcesList"
+                        }
+                    },
+                    "propertyNames": {
+                        "anyOf": [
+                            {
+                                "$ref": "#/definitions/CommonResourcePropertyNames"
+                            },
+                            {
+                                "enum": [
+                                    "list"
+                                ]
+                            }
+                        ]
+                    },
+                    "required": [
+                        "list"
+                    ],
+                    "type": "object"
                 }
             ]
         },
-        "SSHAccessCommonProperties": {
-            "properties": {
-                "connection_port": {
-                    "default": 22,
-                    "description": "Port for SSH-connection to remote machine(s)",
-                    "maximum": 65535,
-                    "minimum": 0,
-                    "type": "integer"
-                },
-                "connection_timeout": {
-                    "default": 10,
-                    "description": "Timeout for SSH-connection to remote machine(s)",
-                    "minimum": 1,
-                    "type": "integer"
-                },
-                "keyfile": {
-                    "description": "Absolute path to keyfile on local machine to access the remote machine(s)",
-                    "type": "string"
-                },
-                "password": {
-                    "description": "Password for SSH-access the remote machine(s)",
-                    "type": "string"
+        "Pods": {
+            "description": "Type of Kubernetes resources. Can be either a list of names or a dictionary with the extra parameters.",
+            "oneOf": [
+                {
+                    "$ref": "#/definitions/PodsList"
                 },
-                "username": {
-                    "default": "root",
-                    "description": "Username for SSH-access the remote machine(s)",
-                    "type": "string"
+                {
+                    "allOf": [
+                        {
+                            "$ref": "#/definitions/CommonResourceProperties"
+                        }
+                    ],
+                    "properties": {
+                        "list": {
+                            "$ref": "#/definitions/PodsList"
+                        },
+                        "namespace": {
+                            "type": "string"
+                        }
+                    },
+                    "propertyNames": {
+                        "anyOf": [
+                            {
+                                "$ref": "#/definitions/CommonResourcePropertyNames"
+                            },
+                            {
+                                "enum": [
+                                    "list",
+                                    "namespace"
+                                ]
+                            }
+                        ]
+                    },
+                    "required": [
+                        "list"
+                    ],
+                    "type": "object"
                 }
-            }
-        },
-        "SSHAccessCommonPropertyNames": {
-            "enum": [
-                "keyfile",
-                "password",
-                "username",
-                "connection_port",
-                "connection_timeout"
             ]
+        },
+        "PodsList": {
+            "$ref": "../../common/utils.json#/definitions/SetOfStrings",
+            "description": "List of pod names"
+        },
+        "ResourcesList": {
+            "description": "List of resource names, or list of dictionaries with the extra parameters",
+            "items": {
+                "oneOf": [
+                    {
+                        "type": "string"
+                    },
+                    {
+                        "additionalProperties": false,
+                        "properties": {
+                            "name": {
+                                "type": "string"
+                            },
+                            "namespace": {
+                                "default": "kube-system",
+                                "type": "string"
+                            }
+                        },
+                        "type": "object"
+                    }
+                ]
+            },
+            "type": "array"
         }
     },
-    "description": "Section to hold the parameters to be applied by default to each record in the nodes section",
-    "propertyNames": {
-        "$ref": "#/definitions/CommonNodePropertyNames"
+    "description": "Wait until the necessary Kubernetes resources are ready",
+    "minProperties": 1,
+    "properties": {
+        "daemonsets": {
+            "$ref": "#/definitions/GenericResource"
+        },
+        "deployments": {
+            "$ref": "#/definitions/GenericResource"
+        },
+        "pods": {
+            "$ref": "#/definitions/Pods"
+        },
+        "replicasets": {
+            "$ref": "#/definitions/GenericResource"
+        },
+        "statefulsets": {
+            "$ref": "#/definitions/GenericResource"
+        }
     },
     "type": "object"
 }
```

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugin_defaults.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugin_defaults.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/calico.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/calico.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999591503267974%*

 * *Differences: {"'properties'": "{'mtu': {'default': 1430}}"}*

```diff
@@ -204,15 +204,15 @@
             "enum": [
                 "ipip",
                 "vxlan",
                 "none"
             ]
         },
         "mtu": {
-            "default": 1440,
+            "default": 1430,
             "description": "MTU size for Calico interface",
             "type": "integer"
         },
         "natOutgoing": {
             "default": true,
             "type": "boolean"
         },
```

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/generic_plugin.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/generic_plugin.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/installation/ansible.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/installation/ansible.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/installation/config.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/installation/config.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/installation/expect.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/installation/template.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.25%*

 * *Differences: {"'definitions'": "{replace: OrderedDict([('Properties', OrderedDict([('properties', "*

 * *                  "OrderedDict([('source', OrderedDict([('type', 'string'), ('description', 'The "*

 * *                  'local path to the source Jinja2 template file. It is compiled before uploading '*

 * *                  "to hosts.')])), ('destination', OrderedDict([('type', 'string'), "*

 * *                  "('description', 'The absolute path on the hosts where the compiled template "*

 * *                  "needs to be uploaded')]) […]*

```diff
@@ -1,150 +1,80 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema",
-    "additionalProperties": false,
     "definitions": {
-        "CommonResourceProperties": {
+        "Properties": {
             "properties": {
-                "retries": {
-                    "default": 30,
-                    "description": "The number of attempts to check the status",
-                    "type": "integer"
-                },
-                "timeout": {
-                    "default": 5,
-                    "description": "The number of seconds until the next resource status check",
-                    "type": "integer"
+                "apply_command": {
+                    "description": "The command to apply the template on remote hosts after uploading it. It is called only if the switch apply_required is on.",
+                    "type": "string"
+                },
+                "apply_groups": {
+                    "$ref": "../../common/node_ref.json#/definitions/Roles",
+                    "description": "List of groups on which the template apply command needs to be executed"
+                },
+                "apply_nodes": {
+                    "$ref": "../../common/node_ref.json#/definitions/Names",
+                    "description": "List of nodes on which the template apply command needs to be executed"
+                },
+                "apply_required": {
+                    "default": true,
+                    "description": "A switch to call the command to apply the uploaded template on remote hosts",
+                    "type": "boolean"
+                },
+                "destination": {
+                    "description": "The absolute path on the hosts where the compiled template needs to be uploaded",
+                    "type": "string"
+                },
+                "destination_groups": {
+                    "$ref": "../../common/node_ref.json#/definitions/Roles",
+                    "description": "List of groups on which the compiled template needs to be uploaded"
+                },
+                "destination_nodes": {
+                    "$ref": "../../common/node_ref.json#/definitions/Names",
+                    "description": "List of nodes on which the compiled template needs to be uploaded"
+                },
+                "source": {
+                    "description": "The local path to the source Jinja2 template file. It is compiled before uploading to hosts.",
+                    "type": "string"
+                },
+                "sudo": {
+                    "default": true,
+                    "description": "A switch for the command execution from the sudoer",
+                    "type": "boolean"
                 }
             }
         },
-        "CommonResourcePropertyNames": {
+        "PropertyNames": {
             "enum": [
-                "timeout",
-                "retries"
-            ]
-        },
-        "GenericResource": {
-            "description": "Type of Kubernetes resources. Can be either a list of names or a dictionary with the extra parameters.",
-            "oneOf": [
-                {
-                    "$ref": "#/definitions/ResourcesList"
-                },
-                {
-                    "allOf": [
-                        {
-                            "$ref": "#/definitions/CommonResourceProperties"
-                        }
-                    ],
-                    "properties": {
-                        "list": {
-                            "$ref": "#/definitions/ResourcesList"
-                        }
-                    },
-                    "propertyNames": {
-                        "anyOf": [
-                            {
-                                "$ref": "#/definitions/CommonResourcePropertyNames"
-                            },
-                            {
-                                "enum": [
-                                    "list"
-                                ]
-                            }
-                        ]
-                    },
-                    "required": [
-                        "list"
-                    ],
-                    "type": "object"
-                }
+                "source",
+                "destination",
+                "apply_required",
+                "apply_command",
+                "sudo",
+                "destination_groups",
+                "destination_nodes",
+                "apply_groups",
+                "apply_nodes"
             ]
+        }
+    },
+    "description": "Compile the Jinja2 template file, upload to remote hosts, and apply it. Can be either a local path to file or a dictionary with the extra parameters.",
+    "oneOf": [
+        {
+            "type": "string"
         },
-        "Pods": {
-            "description": "Type of Kubernetes resources. Can be either a list of names or a dictionary with the extra parameters.",
-            "oneOf": [
-                {
-                    "$ref": "#/definitions/PodsList"
-                },
+        {
+            "allOf": [
                 {
-                    "allOf": [
-                        {
-                            "$ref": "#/definitions/CommonResourceProperties"
-                        }
-                    ],
-                    "properties": {
-                        "list": {
-                            "$ref": "#/definitions/PodsList"
-                        },
-                        "namespace": {
-                            "type": "string"
-                        }
-                    },
-                    "propertyNames": {
-                        "anyOf": [
-                            {
-                                "$ref": "#/definitions/CommonResourcePropertyNames"
-                            },
-                            {
-                                "enum": [
-                                    "list",
-                                    "namespace"
-                                ]
-                            }
-                        ]
-                    },
-                    "required": [
-                        "list"
-                    ],
-                    "type": "object"
+                    "$ref": "#/definitions/Properties"
                 }
-            ]
-        },
-        "PodsList": {
-            "$ref": "../../common/utils.json#/definitions/SetOfStrings",
-            "description": "List of pod names"
-        },
-        "ResourcesList": {
-            "description": "List of resource names, or list of dictionaries with the extra parameters",
-            "items": {
-                "oneOf": [
-                    {
-                        "type": "string"
-                    },
-                    {
-                        "additionalProperties": false,
-                        "properties": {
-                            "name": {
-                                "type": "string"
-                            },
-                            "namespace": {
-                                "default": "kube-system",
-                                "type": "string"
-                            }
-                        },
-                        "type": "object"
-                    }
-                ]
+            ],
+            "propertyNames": {
+                "$ref": "#/definitions/PropertyNames"
             },
-            "type": "array"
+            "required": [
+                "source"
+            ],
+            "type": "object"
         }
-    },
-    "description": "Wait until the necessary Kubernetes resources are ready",
-    "minProperties": 1,
-    "properties": {
-        "daemonsets": {
-            "$ref": "#/definitions/GenericResource"
-        },
-        "deployments": {
-            "$ref": "#/definitions/GenericResource"
-        },
-        "pods": {
-            "$ref": "#/definitions/Pods"
-        },
-        "replicasets": {
-            "$ref": "#/definitions/GenericResource"
-        },
-        "statefulsets": {
-            "$ref": "#/definitions/GenericResource"
-        }
-    },
-    "type": "object"
+    ]
 }
```

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/installation/helm.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/installation/helm.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/installation/python.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/installation/python.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/installation/shell.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/installation/shell.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/installation/template.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/thirdparties.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.2857142857142857%*

 * *Differences: {"'additionalProperties'": "OrderedDict([('$ref', '#/definitions/ThirdParty')])",*

 * * "'definitions'": "{replace: OrderedDict([('MinimalThirdPartyProperties', "*

 * *                  "OrderedDict([('properties', OrderedDict([('source', OrderedDict([('type', "*

 * *                  "'string'), ('description', 'Source from where to upload the file to hosts. It "*

 * *                  "can be an URL or an absolute path on the deployment node.')])), ('sha1', "*

 * *                  "OrderedDict([('type', 'string'), ('description' […]*

```diff
@@ -1,80 +1,120 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema",
+    "additionalProperties": {
+        "$ref": "#/definitions/ThirdParty"
+    },
     "definitions": {
-        "Properties": {
+        "MinimalThirdPartyProperties": {
             "properties": {
-                "apply_command": {
-                    "description": "The command to apply the template on remote hosts after uploading it. It is called only if the switch apply_required is on.",
-                    "type": "string"
-                },
-                "apply_groups": {
-                    "$ref": "../../common/node_ref.json#/definitions/Roles",
-                    "description": "List of groups on which the template apply command needs to be executed"
-                },
-                "apply_nodes": {
-                    "$ref": "../../common/node_ref.json#/definitions/Names",
-                    "description": "List of nodes on which the template apply command needs to be executed"
-                },
-                "apply_required": {
-                    "default": true,
-                    "description": "A switch to call the command to apply the uploaded template on remote hosts",
-                    "type": "boolean"
-                },
-                "destination": {
-                    "description": "The absolute path on the hosts where the compiled template needs to be uploaded",
+                "sha1": {
+                    "description": "SHA1 hash of the file. It is necessary in order to check with an existing file on the hosts and decide whether to download the file or not.",
                     "type": "string"
                 },
-                "destination_groups": {
-                    "$ref": "../../common/node_ref.json#/definitions/Roles",
-                    "description": "List of groups on which the compiled template needs to be uploaded"
-                },
-                "destination_nodes": {
-                    "$ref": "../../common/node_ref.json#/definitions/Names",
-                    "description": "List of nodes on which the compiled template needs to be uploaded"
-                },
                 "source": {
-                    "description": "The local path to the source Jinja2 template file. It is compiled before uploading to hosts.",
+                    "description": "Source from where to upload the file to hosts. It can be an URL or an absolute path on the deployment node.",
                     "type": "string"
-                },
-                "sudo": {
-                    "default": true,
-                    "description": "A switch for the command execution from the sudoer",
-                    "type": "boolean"
                 }
             }
         },
-        "PropertyNames": {
+        "MinimalThirdPartyPropertyNames": {
             "enum": [
                 "source",
-                "destination",
-                "apply_required",
-                "apply_command",
-                "sudo",
-                "destination_groups",
-                "destination_nodes",
-                "apply_groups",
-                "apply_nodes"
+                "sha1"
             ]
-        }
-    },
-    "description": "Compile the Jinja2 template file, upload to remote hosts, and apply it. Can be either a local path to file or a dictionary with the extra parameters.",
-    "oneOf": [
-        {
-            "type": "string"
         },
-        {
-            "allOf": [
+        "ThirdParty": {
+            "description": "The absolute destination path of the 3rd-party on the host system of the cluster",
+            "oneOf": [
                 {
-                    "$ref": "#/definitions/Properties"
+                    "type": "string"
+                },
+                {
+                    "allOf": [
+                        {
+                            "$ref": "#/definitions/MinimalThirdPartyProperties"
+                        }
+                    ],
+                    "properties": {
+                        "group": {
+                            "$ref": "../common/node_ref.json#/definitions/Role",
+                            "description": "The name of the group to whose hosts the file should be uploaded"
+                        },
+                        "groups": {
+                            "$ref": "../common/node_ref.json#/definitions/Roles",
+                            "description": "The list of group names to whose hosts the file should be uploaded"
+                        },
+                        "mode": {
+                            "default": "700",
+                            "description": "The mode which needs to be assigned to the file after downloading it",
+                            "type": [
+                                "string",
+                                "integer"
+                            ]
+                        },
+                        "node": {
+                            "$ref": "../common/node_ref.json#/definitions/Name",
+                            "description": "The name of node where the file should be uploaded"
+                        },
+                        "nodes": {
+                            "$ref": "../common/node_ref.json#/definitions/Names",
+                            "description": "The list of node names where the file should be uploaded"
+                        },
+                        "owner": {
+                            "default": "root",
+                            "description": "The owner who needs to be assigned to the file after downloading it",
+                            "type": "string"
+                        },
+                        "unpack": {
+                            "description": "Absolute path on hosts where to unpack the downloaded file. Unpacking is supported only for the following file extensions: .tar, .gz and .zip.",
+                            "type": "string"
+                        }
+                    },
+                    "propertyNames": {
+                        "anyOf": [
+                            {
+                                "$ref": "#/definitions/MinimalThirdPartyPropertyNames"
+                            },
+                            {
+                                "enum": [
+                                    "owner",
+                                    "mode",
+                                    "unpack",
+                                    "group",
+                                    "groups",
+                                    "node",
+                                    "nodes"
+                                ]
+                            }
+                        ]
+                    },
+                    "required": [
+                        "source"
+                    ],
+                    "type": "object"
                 }
-            ],
-            "propertyNames": {
-                "$ref": "#/definitions/PropertyNames"
-            },
-            "required": [
-                "source"
-            ],
-            "type": "object"
+            ]
         }
-    ]
+    },
+    "description": "Deliver files from third party sources and install them in the system",
+    "properties": {
+        "/usr/bin/calicoctl": {
+            "$ref": "#/definitions/ThirdParty"
+        },
+        "/usr/bin/crictl.tar.gz": {
+            "$ref": "#/definitions/ThirdParty"
+        },
+        "/usr/bin/etcdctl": {
+            "$ref": "#/definitions/ThirdParty"
+        },
+        "/usr/bin/kubeadm": {
+            "$ref": "#/definitions/ThirdParty"
+        },
+        "/usr/bin/kubectl": {
+            "$ref": "#/definitions/ThirdParty"
+        },
+        "/usr/bin/kubelet": {
+            "$ref": "#/definitions/ThirdParty"
+        }
+    },
+    "type": "object"
 }
```

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/installation.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/installation.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/kubernetes-dashboard.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/kubernetes-dashboard.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/local-path-provisioner.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/local-path-provisioner.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/nginx-ingress-controller.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/nginx-ingress-controller.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/procedures.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/procedures.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/rbac/account.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/rbac/account.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/rbac/account_defaults.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/rbac/account_defaults.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/rbac/psp.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/rbac/psp.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/rbac/pss.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/rbac/pss.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/rbac.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/rbac.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/registry.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/registry.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/audit.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/audit.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/coredns.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/coredns.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/cri.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/cri.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/etc_hosts.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/etc_hosts.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/kernel_security.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/kernel_security.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/kubeadm.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/kubeadm.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/kubeadm_kube-proxy.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/kubeadm_kube-proxy.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/kubeadm_kubelet.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/kubeadm_kubelet.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/kubeadm_patches.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/kubeadm_patches.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/loadbalancer.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/loadbalancer.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/modprobe.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/modprobe.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/ntp.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/ntp.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/packages/associations.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/packages/associations.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/packages.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/packages.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/sysctl.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/sysctl.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/thirdparties.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/vrrp_ip.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.21428571428571427%*

 * *Differences: {"'definitions'": "{replace: OrderedDict([('ExtendedVRRP', OrderedDict([('type', 'object'), "*

 * *                  "('properties', OrderedDict([('ip', OrderedDict([('type', 'string'), "*

 * *                  "('description', 'The IP address for virtual IP')])), ('floating_ip', "*

 * *                  "OrderedDict([('type', 'string'), ('description', 'The floating IP address for "*

 * *                  "virtual IP')])), ('hosts', OrderedDict([('type', 'array'), ('description', "*

 * *                  "'List of hosts on which t […]*

```diff
@@ -1,120 +1,103 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema",
-    "additionalProperties": {
-        "$ref": "#/definitions/ThirdParty"
-    },
     "definitions": {
-        "MinimalThirdPartyProperties": {
+        "ExtendedVRRP": {
+            "additionalProperties": false,
             "properties": {
-                "sha1": {
-                    "description": "SHA1 hash of the file. It is necessary in order to check with an existing file on the hosts and decide whether to download the file or not.",
+                "control_endpoint": {
+                    "default": false,
+                    "description": "Parameter to help the algorithm in choosing which address to take as the control_plain",
+                    "type": "boolean"
+                },
+                "floating_ip": {
+                    "description": "The floating IP address for virtual IP",
+                    "type": "string"
+                },
+                "hosts": {
+                    "description": "List of hosts on which the VRRP IP should be set. Each item can be either a name of the balancer node, or a dictionary with the balancer name and additional parameters.",
+                    "items": {
+                        "$ref": "#/definitions/HostToApplyVRRP"
+                    },
+                    "type": "array"
+                },
+                "id": {
+                    "description": "The ID of the VRRP IP. It must be unique for each VRRP IP.",
+                    "type": "string"
+                },
+                "interface": {
+                    "default": "auto",
+                    "description": "The interface on which the address must be listened. The value of this property is propagated to the corresponding hosts[i].interface property, if the latter is not explicitly defined.",
+                    "type": "string"
+                },
+                "ip": {
+                    "description": "The IP address for virtual IP",
+                    "type": "string"
+                },
+                "params": {
+                    "additionalProperties": false,
+                    "description": "Additional params for other non-keepalived services",
+                    "properties": {
+                        "maintenance-type": {
+                            "description": "Label for IPs that describes what type of traffic should be received in maintenance mode",
+                            "enum": [
+                                "not bind"
+                            ]
+                        }
+                    },
+                    "type": "object"
+                },
+                "password": {
+                    "description": "Password for VRRP IP set. It must be unique for every VRRP IP ID.",
                     "type": "string"
                 },
-                "source": {
-                    "description": "Source from where to upload the file to hosts. It can be an URL or an absolute path on the deployment node.",
+                "router_id": {
+                    "description": "The router ID of the VRRP IP. Must be unique for each VRRP IP ID and have maximum 3-character size.",
                     "type": "string"
                 }
-            }
+            },
+            "required": [
+                "ip"
+            ],
+            "type": "object"
         },
-        "MinimalThirdPartyPropertyNames": {
-            "enum": [
-                "source",
-                "sha1"
-            ]
-        },
-        "ThirdParty": {
-            "description": "The absolute destination path of the 3rd-party on the host system of the cluster",
+        "HostToApplyVRRP": {
             "oneOf": [
                 {
                     "type": "string"
                 },
                 {
-                    "allOf": [
-                        {
-                            "$ref": "#/definitions/MinimalThirdPartyProperties"
-                        }
-                    ],
+                    "additionalProperties": false,
                     "properties": {
-                        "group": {
-                            "$ref": "../common/node_ref.json#/definitions/Role",
-                            "description": "The name of the group to whose hosts the file should be uploaded"
-                        },
-                        "groups": {
-                            "$ref": "../common/node_ref.json#/definitions/Roles",
-                            "description": "The list of group names to whose hosts the file should be uploaded"
-                        },
-                        "mode": {
-                            "default": "700",
-                            "description": "The mode which needs to be assigned to the file after downloading it",
-                            "type": [
-                                "string",
-                                "integer"
-                            ]
-                        },
-                        "node": {
-                            "$ref": "../common/node_ref.json#/definitions/Name",
-                            "description": "The name of node where the file should be uploaded"
-                        },
-                        "nodes": {
-                            "$ref": "../common/node_ref.json#/definitions/Names",
-                            "description": "The list of node names where the file should be uploaded"
-                        },
-                        "owner": {
-                            "default": "root",
-                            "description": "The owner who needs to be assigned to the file after downloading it",
+                        "interface": {
+                            "default": "auto",
+                            "description": "The interface on which the address must be listened for the particular host",
                             "type": "string"
                         },
-                        "unpack": {
-                            "description": "Absolute path on hosts where to unpack the downloaded file. Unpacking is supported only for the following file extensions: .tar, .gz and .zip.",
+                        "name": {
+                            "description": "The name of the node. It must match the name in the nodes list.",
                             "type": "string"
+                        },
+                        "priority": {
+                            "description": "The priority of the VRRP IP host",
+                            "maximum": 255,
+                            "minimum": 0,
+                            "type": "integer"
                         }
                     },
-                    "propertyNames": {
-                        "anyOf": [
-                            {
-                                "$ref": "#/definitions/MinimalThirdPartyPropertyNames"
-                            },
-                            {
-                                "enum": [
-                                    "owner",
-                                    "mode",
-                                    "unpack",
-                                    "group",
-                                    "groups",
-                                    "node",
-                                    "nodes"
-                                ]
-                            }
-                        ]
-                    },
                     "required": [
-                        "source"
+                        "name"
                     ],
                     "type": "object"
                 }
             ]
         }
     },
-    "description": "Deliver files from third party sources and install them in the system",
-    "properties": {
-        "/usr/bin/calicoctl": {
-            "$ref": "#/definitions/ThirdParty"
-        },
-        "/usr/bin/crictl.tar.gz": {
-            "$ref": "#/definitions/ThirdParty"
+    "oneOf": [
+        {
+            "type": "string"
         },
-        "/usr/bin/etcdctl": {
-            "$ref": "#/definitions/ThirdParty"
-        },
-        "/usr/bin/kubeadm": {
-            "$ref": "#/definitions/ThirdParty"
-        },
-        "/usr/bin/kubectl": {
-            "$ref": "#/definitions/ThirdParty"
-        },
-        "/usr/bin/kubelet": {
-            "$ref": "#/definitions/ThirdParty"
+        {
+            "$ref": "#/definitions/ExtendedVRRP"
         }
-    },
-    "type": "object"
+    ]
 }
```

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/vrrp_ip.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/upgrade.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.21428571428571427%*

 * *Differences: {"'additionalProperties'": 'OrderedDict([(\'type\', \'object\'), (\'description\', "Configuration '*

 * *                           'for the upgrade to the particular version from the \'upgrade_plan\'"), '*

 * *                           "('properties', OrderedDict([('thirdparties', OrderedDict([('$ref', "*

 * *                           "'definitions/services/thirdparties.json')])), ('packages', "*

 * *                           "OrderedDict([('type', 'object'), ('description', 'Section for packages "*

 * *                         […]*

```diff
@@ -1,103 +1,129 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema",
-    "definitions": {
-        "ExtendedVRRP": {
-            "additionalProperties": false,
-            "properties": {
-                "control_endpoint": {
-                    "default": false,
-                    "description": "Parameter to help the algorithm in choosing which address to take as the control_plain",
-                    "type": "boolean"
-                },
-                "floating_ip": {
-                    "description": "The floating IP address for virtual IP",
-                    "type": "string"
-                },
-                "hosts": {
-                    "description": "List of hosts on which the VRRP IP should be set. Each item can be either a name of the balancer node, or a dictionary with the balancer name and additional parameters.",
-                    "items": {
-                        "$ref": "#/definitions/HostToApplyVRRP"
-                    },
-                    "type": "array"
-                },
-                "id": {
-                    "description": "The ID of the VRRP IP. It must be unique for each VRRP IP.",
-                    "type": "string"
-                },
-                "interface": {
-                    "default": "auto",
-                    "description": "The interface on which the address must be listened. The value of this property is propagated to the corresponding hosts[i].interface property, if the latter is not explicitly defined.",
-                    "type": "string"
+    "additionalProperties": {
+        "additionalProperties": false,
+        "description": "Configuration for the upgrade to the particular version from the 'upgrade_plan'",
+        "properties": {
+            "cri": {
+                "additionalProperties": false,
+                "description": "Configure container runtime used for Kubernetes",
+                "properties": {
+                    "containerdConfig": {
+                        "$ref": "#/definitions/ContainerdConfig"
+                    }
                 },
-                "ip": {
-                    "description": "The IP address for virtual IP",
-                    "type": "string"
+                "type": "object"
+            },
+            "packages": {
+                "allOf": [
+                    {
+                        "$ref": "definitions/services/packages.json#/definitions/CustomPackages"
+                    }
+                ],
+                "description": "Section for packages and their management during upgrade",
+                "properties": {
+                    "associations": {
+                        "additionalProperties": false,
+                        "description": "Configure associations of package objects to be used during upgrade",
+                        "properties": {
+                            "containerd": {
+                                "$ref": "definitions/services/packages/associations.json#/definitions/PackageNameOnlyAssociations"
+                            },
+                            "docker": {
+                                "$ref": "definitions/services/packages/associations.json#/definitions/PackageNameOnlyAssociations"
+                            }
+                        },
+                        "type": "object"
+                    }
                 },
-                "params": {
-                    "additionalProperties": false,
-                    "description": "Additional params for other non-keepalived services",
-                    "properties": {
-                        "maintenance-type": {
-                            "description": "Label for IPs that describes what type of traffic should be received in maintenance mode",
+                "propertyNames": {
+                    "anyOf": [
+                        {
+                            "$ref": "definitions/services/packages.json#/definitions/CustomPackagesPropertyNames"
+                        },
+                        {
                             "enum": [
-                                "not bind"
+                                "associations"
                             ]
                         }
-                    },
-                    "type": "object"
+                    ]
                 },
-                "password": {
-                    "description": "Password for VRRP IP set. It must be unique for every VRRP IP ID.",
-                    "type": "string"
-                },
-                "router_id": {
-                    "description": "The router ID of the VRRP IP. Must be unique for each VRRP IP ID and have maximum 3-character size.",
-                    "type": "string"
-                }
+                "type": "object"
             },
-            "required": [
-                "ip"
-            ],
-            "type": "object"
+            "plugins": {
+                "$ref": "definitions/plugins.json"
+            },
+            "thirdparties": {
+                "$ref": "definitions/services/thirdparties.json"
+            }
         },
-        "HostToApplyVRRP": {
-            "oneOf": [
-                {
-                    "type": "string"
-                },
-                {
+        "type": "object"
+    },
+    "definitions": {
+        "ContainerdConfig": {
+            "additionalProperties": false,
+            "description": "Parameters for containerd passed to config.toml",
+            "properties": {
+                "plugins.\"io.containerd.grpc.v1.cri\"": {
                     "additionalProperties": false,
                     "properties": {
-                        "interface": {
-                            "default": "auto",
-                            "description": "The interface on which the address must be listened for the particular host",
+                        "sandbox_image": {
                             "type": "string"
-                        },
-                        "name": {
-                            "description": "The name of the node. It must match the name in the nodes list.",
-                            "type": "string"
-                        },
-                        "priority": {
-                            "description": "The priority of the VRRP IP host",
-                            "maximum": 255,
-                            "minimum": 0,
-                            "type": "integer"
                         }
                     },
-                    "required": [
-                        "name"
-                    ],
                     "type": "object"
                 }
-            ]
+            },
+            "type": "object"
         }
     },
-    "oneOf": [
-        {
-            "type": "string"
+    "properties": {
+        "disable-eviction": {
+            "$ref": "definitions/procedures.json#/definitions/DisableEviction"
+        },
+        "drain_timeout": {
+            "$ref": "definitions/procedures.json#/definitions/DrainTimeout"
+        },
+        "grace_period": {
+            "$ref": "definitions/procedures.json#/definitions/GracePeriod"
         },
-        {
-            "$ref": "#/definitions/ExtendedVRRP"
+        "prepull_group_size": {
+            "$ref": "definitions/procedures.json#/definitions/PrepullGroupSize"
+        },
+        "upgrade_nodes": {
+            "description": "Manually specify certain nodes that need to be upgraded. Each item can be either a node name referring to the cluster.yaml, or full node specification.",
+            "items": {
+                "oneOf": [
+                    {
+                        "$ref": "definitions/common/node_ref.json#/definitions/Name"
+                    },
+                    {
+                        "allOf": [
+                            {
+                                "$ref": "definitions/node.json#/definitions/Properties"
+                            }
+                        ],
+                        "propertyNames": {
+                            "$ref": "definitions/node.json#/definitions/PropertyNames"
+                        },
+                        "required": [
+                            "name"
+                        ],
+                        "type": "object"
+                    }
+                ]
+            },
+            "minItems": 1,
+            "type": "array",
+            "uniqueItems": true
+        },
+        "upgrade_plan": {
+            "$ref": "definitions/common/utils.json#/definitions/NonEmptySetOfStrings",
+            "description": "List of new versions through which to upgrade the cluster to the last specified version"
         }
-    ]
+    },
+    "required": [
+        "upgrade_plan"
+    ],
+    "type": "object"
 }
```

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/manage_psp.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/manage_psp.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/manage_pss.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/manage_pss.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/migrate_cri.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/migrate_cri.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/migrate_kubemarine.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/migrate_kubemarine.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/reboot.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/reboot.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/reconfigure.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/reconfigure.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/remove_node.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/remove_node.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/restore.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/restore.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/schemas/upgrade.json` & `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/node_defaults.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.2777777777777778%*

 * *Differences: {"'allOf'": "[OrderedDict([('$ref', '#/definitions/CommonNodeProperties')])]",*

 * * "'definitions'": "{replace: OrderedDict([('SSHAccessCommonProperties', "*

 * *                  "OrderedDict([('properties', OrderedDict([('keyfile', OrderedDict([('type', "*

 * *                  "'string'), ('description', 'Absolute path to keyfile on local machine to access "*

 * *                  "the remote machine(s)')])), ('password', OrderedDict([('type', 'string'), "*

 * *                  "('description', 'Password for SSH-access the rem […]*

```diff
@@ -1,129 +1,156 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema",
-    "additionalProperties": {
-        "additionalProperties": false,
-        "description": "Configuration for the upgrade to the particular version from the 'upgrade_plan'",
-        "properties": {
-            "cri": {
-                "additionalProperties": false,
-                "description": "Configure container runtime used for Kubernetes",
-                "properties": {
-                    "containerdConfig": {
-                        "$ref": "#/definitions/ContainerdConfig"
-                    }
-                },
-                "type": "object"
-            },
-            "packages": {
-                "allOf": [
-                    {
-                        "$ref": "definitions/services/packages.json#/definitions/CustomPackages"
-                    }
-                ],
-                "description": "Section for packages and their management during upgrade",
-                "properties": {
-                    "associations": {
-                        "additionalProperties": false,
-                        "description": "Configure associations of package objects to be used during upgrade",
-                        "properties": {
-                            "containerd": {
-                                "$ref": "definitions/services/packages/associations.json#/definitions/PackageNameOnlyAssociations"
-                            },
-                            "docker": {
-                                "$ref": "definitions/services/packages/associations.json#/definitions/PackageNameOnlyAssociations"
-                            }
-                        },
-                        "type": "object"
-                    }
-                },
-                "propertyNames": {
-                    "anyOf": [
-                        {
-                            "$ref": "definitions/services/packages.json#/definitions/CustomPackagesPropertyNames"
-                        },
-                        {
-                            "enum": [
-                                "associations"
-                            ]
+    "allOf": [
+        {
+            "$ref": "#/definitions/CommonNodeProperties"
+        }
+    ],
+    "definitions": {
+        "CommonNodeAccessProperties": {
+            "allOf": [
+                {
+                    "$ref": "#/definitions/SSHAccessCommonProperties"
+                }
+            ],
+            "properties": {
+                "boot": {
+                    "additionalProperties": false,
+                    "description": "Nodes boot settings",
+                    "properties": {
+                        "timeout": {
+                            "default": 600,
+                            "description": "Timeout for node reboot in seconds",
+                            "minimal": 1,
+                            "type": "integer"
                         }
-                    ]
+                    },
+                    "type": "object"
                 },
-                "type": "object"
-            },
-            "plugins": {
-                "$ref": "definitions/plugins.json"
-            },
-            "thirdparties": {
-                "$ref": "definitions/services/thirdparties.json"
+                "gateway": {
+                    "description": "Gateway that should be used to connect to node(s)",
+                    "type": "string"
+                }
             }
         },
-        "type": "object"
-    },
-    "definitions": {
-        "ContainerdConfig": {
-            "additionalProperties": false,
-            "description": "Parameters for containerd passed to config.toml",
+        "CommonNodeAccessPropertyNames": {
+            "anyOf": [
+                {
+                    "$ref": "#/definitions/SSHAccessCommonPropertyNames"
+                },
+                {
+                    "enum": [
+                        "gateway",
+                        "boot"
+                    ]
+                }
+            ]
+        },
+        "CommonNodeProperties": {
+            "allOf": [
+                {
+                    "$ref": "#/definitions/CommonNodeAccessProperties"
+                }
+            ],
             "properties": {
-                "plugins.\"io.containerd.grpc.v1.cri\"": {
-                    "additionalProperties": false,
+                "labels": {
+                    "additionalProperties": {
+                        "type": [
+                            "string",
+                            "boolean",
+                            "integer"
+                        ]
+                    },
+                    "description": "Additional labels for node(s)",
+                    "type": "object"
+                },
+                "taints": {
+                    "$ref": "common/utils.json#/definitions/ArrayOfStrings",
+                    "description": "Additional taints for node(s). Caution: Use at your own risk. It can cause unexpected behavior. No support is provided for consequences."
+                }
+            }
+        },
+        "CommonNodePropertyNames": {
+            "anyOf": [
+                {
+                    "$ref": "#/definitions/CommonNodeAccessPropertyNames"
+                },
+                {
+                    "enum": [
+                        "labels",
+                        "taints"
+                    ]
+                }
+            ]
+        },
+        "OneOfKeyfilePasswordSpec": {
+            "oneOf": [
+                {
+                    "properties": {
+                        "keyfile": {
+                            "type": "string"
+                        }
+                    },
+                    "required": [
+                        "keyfile"
+                    ],
+                    "type": "object"
+                },
+                {
                     "properties": {
-                        "sandbox_image": {
+                        "password": {
                             "type": "string"
                         }
                     },
+                    "required": [
+                        "password"
+                    ],
                     "type": "object"
                 }
-            },
-            "type": "object"
+            ]
+        },
+        "SSHAccessCommonProperties": {
+            "properties": {
+                "connection_port": {
+                    "default": 22,
+                    "description": "Port for SSH-connection to remote machine(s)",
+                    "maximum": 65535,
+                    "minimum": 0,
+                    "type": "integer"
+                },
+                "connection_timeout": {
+                    "default": 10,
+                    "description": "Timeout for SSH-connection to remote machine(s)",
+                    "minimum": 1,
+                    "type": "integer"
+                },
+                "keyfile": {
+                    "description": "Absolute path to keyfile on local machine to access the remote machine(s)",
+                    "type": "string"
+                },
+                "password": {
+                    "description": "Password for SSH-access the remote machine(s)",
+                    "type": "string"
+                },
+                "username": {
+                    "default": "root",
+                    "description": "Username for SSH-access the remote machine(s)",
+                    "type": "string"
+                }
+            }
+        },
+        "SSHAccessCommonPropertyNames": {
+            "enum": [
+                "keyfile",
+                "password",
+                "username",
+                "connection_port",
+                "connection_timeout"
+            ]
         }
     },
-    "properties": {
-        "disable-eviction": {
-            "$ref": "definitions/procedures.json#/definitions/DisableEviction"
-        },
-        "drain_timeout": {
-            "$ref": "definitions/procedures.json#/definitions/DrainTimeout"
-        },
-        "grace_period": {
-            "$ref": "definitions/procedures.json#/definitions/GracePeriod"
-        },
-        "prepull_group_size": {
-            "$ref": "definitions/procedures.json#/definitions/PrepullGroupSize"
-        },
-        "upgrade_nodes": {
-            "description": "Manually specify certain nodes that need to be upgraded. Each item can be either a node name referring to the cluster.yaml, or full node specification.",
-            "items": {
-                "oneOf": [
-                    {
-                        "$ref": "definitions/common/node_ref.json#/definitions/Name"
-                    },
-                    {
-                        "allOf": [
-                            {
-                                "$ref": "definitions/node.json#/definitions/Properties"
-                            }
-                        ],
-                        "propertyNames": {
-                            "$ref": "definitions/node.json#/definitions/PropertyNames"
-                        },
-                        "required": [
-                            "name"
-                        ],
-                        "type": "object"
-                    }
-                ]
-            },
-            "minItems": 1,
-            "type": "array",
-            "uniqueItems": true
-        },
-        "upgrade_plan": {
-            "$ref": "definitions/common/utils.json#/definitions/NonEmptySetOfStrings",
-            "description": "List of new versions through which to upgrade the cluster to the last specified version"
-        }
+    "description": "Section to hold the parameters to be applied by default to each record in the nodes section",
+    "propertyNames": {
+        "$ref": "#/definitions/CommonNodePropertyNames"
     },
-    "required": [
-        "upgrade_plan"
-    ],
     "type": "object"
 }
```

### Comparing `kubemarine-0.28.1/kubemarine/resources/scripts/__init__.py` & `kubemarine-0.29.0/kubemarine/resources/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/scripts/check_url_availability.py` & `kubemarine-0.29.0/kubemarine/resources/scripts/check_url_availability.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,35 +12,44 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # Check url availability script.
 # The script is for testing purpose only.
 # The first argv parameter is source. The second argv parameter is the timeout.
 
+import ssl
 import sys
 
 major_version = sys.version_info.major
 if major_version == 3:
     import urllib.request as urllib
     import urllib.parse as urlparse
 else:
+    # pylint: disable-next=import-error
     import urllib2 as urllib  # type: ignore[import-not-found, no-redef]
-    import urlparse as urlparse # type: ignore[import-not-found, no-redef]
+    # pylint: disable-next=import-error
+    import urlparse  # type: ignore[import-not-found, no-redef]
 
 try:
     source = sys.argv[1]
     timeout = int(sys.argv[2])
     parsed_url = urlparse.urlparse(source)
     no_auth_netloc = parsed_url.netloc.split('@')[-1]
     no_auth_url = parsed_url._replace(netloc="{}".format(no_auth_netloc)).geturl()
 
     password_mgr = urllib.HTTPPasswordMgrWithDefaultRealm()
     password_mgr.add_password(None, no_auth_url, parsed_url.username or '', parsed_url.password or '')
-    handler = urllib.HTTPBasicAuthHandler(password_mgr)
-    opener = urllib.build_opener(handler)
+    basic_auth_handler = urllib.HTTPBasicAuthHandler(password_mgr)
+
+    ssl_ctx = ssl.create_default_context()
+    ssl_ctx.check_hostname = False
+    ssl_ctx.verify_mode = ssl.CERT_NONE
+    https_handler = urllib.HTTPSHandler(context=ssl_ctx)
+
+    opener = urllib.build_opener(https_handler, basic_auth_handler)
 
     status_code = opener.open(no_auth_url, timeout=timeout).getcode()
     if status_code != 200:
         sys.stderr.write("Error status code: %s" % status_code)
         sys.exit(1)
 except Exception as e:
     sys.stderr.write(str(e))
```

### Comparing `kubemarine-0.28.1/kubemarine/resources/scripts/etcdctl.sh` & `kubemarine-0.29.0/kubemarine/resources/scripts/etcdctl.sh`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/scripts/simple_port_client.py` & `kubemarine-0.29.0/kubemarine/resources/scripts/simple_port_client.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/scripts/simple_port_listener.py` & `kubemarine-0.29.0/kubemarine/resources/scripts/simple_port_listener.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/scripts/source/ipip_check/go.sum` & `kubemarine-0.29.0/kubemarine/resources/scripts/source/ipip_check/go.sum`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/resources/scripts/source/ipip_check/ipip_check.go` & `kubemarine-0.29.0/kubemarine/resources/scripts/source/ipip_check/ipip_check.go`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/selinux.py` & `kubemarine-0.29.0/kubemarine/selinux.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import io
 import re
 from typing import Tuple, Optional, Dict, List
 
-from kubemarine import system
 from kubemarine.core import utils, log
 from kubemarine.core.group import NodeGroup, RunnersGroupResult
 
 # Common regexp should support the following schemes:
 # SELinux status:                 enabled
 # SELinuxfs mount:                /selinux
 # Policy version:                 23
@@ -172,29 +171,32 @@
             # if break was called in previous for loop, then do break in current loop
             break
 
     return valid, result, parsed_result
 
 
 def setup_selinux(group: NodeGroup) -> Optional[RunnersGroupResult]:
+    from kubemarine import system  # pylint: disable=cyclic-import
+
     log = group.cluster.log
 
     # this method handles cluster with multiple os, suppressing should be enabled
     if group.get_nodes_os() not in ['rhel', 'rhel8', 'rhel9']:
         log.debug("Skipped - selinux is not supported on Ubuntu/Debian os family")
         return None
 
     expected_state = get_expected_state(group.cluster.inventory)
     expected_policy = get_expected_policy(group.cluster.inventory)
     expected_permissive = get_expected_permissive(group.cluster.inventory)
 
-    valid, result, parsed_result = is_config_valid(group,
-                                                   state=expected_state,
-                                                   policy=expected_policy,
-                                                   permissive=expected_permissive)
+    valid, result, _ = \
+        is_config_valid(group,
+                        state=expected_state,
+                        policy=expected_policy,
+                        permissive=expected_permissive)
 
     if valid:
         log.debug("Skipped - selinux already correctly configured")
         return result
 
     config = io.StringIO('SELINUX=%s\nSELINUXTYPE=%s\n' % (expected_state, expected_policy))
```

### Comparing `kubemarine-0.28.1/kubemarine/sysctl.py` & `kubemarine-0.29.0/kubemarine/sysctl.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/system.py` & `kubemarine-0.29.0/kubemarine/system.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import configparser
 import io
-import paramiko
 import re
 import socket
 import time
 from typing import Dict, Tuple, Optional, List
 
+import paramiko
 from dateutil.parser import parse
 from ordered_set import OrderedSet
 
-from kubemarine import selinux, kubernetes, apparmor, sysctl, modprobe
+from kubemarine import selinux, apparmor, sysctl, modprobe
 from kubemarine.core import utils, static
 from kubemarine.core.cluster import KubernetesCluster, EnrichmentStage, enrichment
 from kubemarine.core.executor import RunnersResult, Token, GenericResult, Callback, RawExecutor
 from kubemarine.core.group import (
     GenericGroupResult, RunnersGroupResult, GroupResultException,
     NodeGroup, DeferredGroup, AbstractGroup, GROUP_RUN_TYPE, CollectorCallback
 )
@@ -89,19 +89,19 @@
     detect_os_family(cluster)
     logger.verbose('OS family check finished')
 
     logger.debug('Detecting nodes context finished!')
 
 
 def fetch_os_versions(cluster: KubernetesCluster) -> RunnersGroupResult:
-    group = cluster.make_group(cluster.nodes_context).get_accessible_nodes()
     '''
     For Red Hat, CentOS, Oracle Linux, and Ubuntu information in /etc/os-release /etc/redhat-release is sufficient but,
     Debian stores the full version in a special file. sed transforms version string, eg 10.10 becomes DEBIAN_VERSION="10.10"  
     '''
+    group = cluster.make_group(cluster.nodes_context).get_accessible_nodes()
 
     return group.run(
         "cat /etc/*elease; cat /etc/debian_version 2> /dev/null | sed 's/\\(.\\+\\)/DEBIAN_VERSION=\"\\1\"/' || true")
 
 
 def detect_os_family(cluster: KubernetesCluster) -> None:
     results = fetch_os_versions(cluster)
@@ -187,16 +187,15 @@
 # generate records for /etc/hosts from services.etc_hosts or services.etc_hosts_generated
 
     result = ""
 
     max_len_ip = 0
 
     for ip in list(inventory['services'][etc_hosts_part].keys()):
-        if len(ip) > max_len_ip:
-            max_len_ip = len(ip)
+        max_len_ip = max(max_len_ip, len(ip))
 
     for ip, names in inventory['services'][etc_hosts_part].items():
         if isinstance(names, list):
             # remove records with empty values from list
             names = list(filter(len, names))
             # if list is empty, then skip
             if not names:
@@ -329,14 +328,16 @@
 
 
 def reboot_nodes(cluster: KubernetesCluster) -> None:
     cluster.get_new_nodes_or_self().call(reboot_group)
 
 
 def reboot_group(group: NodeGroup, try_graceful: bool = None) -> RunnersGroupResult:
+    from kubemarine import kubernetes  # pylint: disable=cyclic-import
+
     cluster: KubernetesCluster = group.cluster
     log = cluster.log
 
     if try_graceful is None:
         if 'controlplain_uri' not in cluster.context.keys():
             kubernetes.is_cluster_installed(cluster)
 
@@ -478,15 +479,15 @@
     group = cluster.get_new_nodes_or_self()
     log = cluster.log
     # this method handles clusters with multiple OS
     os_family = group.get_nodes_os()
 
     if os_family in ['rhel', 'rhel8', 'rhel9'] and cluster.is_task_completed('prepare.system.setup_selinux'):
         log.debug("Verifying Selinux...")
-        selinux_configured, selinux_result, selinux_parsed_result = \
+        selinux_configured, selinux_result, _ = \
             selinux.is_config_valid(group,
                                     state=selinux.get_expected_state(cluster.inventory),
                                     policy=selinux.get_expected_policy(cluster.inventory),
                                     permissive=selinux.get_expected_permissive(cluster.inventory))
         log.debug(selinux_result)
         if not selinux_configured:
             raise Exception("Selinux is still not configured")
```

### Comparing `kubemarine-0.28.1/kubemarine/templates/__init__.py` & `kubemarine-0.29.0/kubemarine/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/templates/admission.yaml.j2` & `kubemarine-0.29.0/kubemarine/templates/admission.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/templates/haproxy.cfg.j2` & `kubemarine-0.29.0/kubemarine/templates/haproxy.cfg.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/templates/keepalived.conf.j2` & `kubemarine-0.29.0/kubemarine/templates/keepalived.conf.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/templates/kubelet.service.j2` & `kubemarine-0.29.0/kubemarine/templates/kubelet.service.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/templates/plugins/__init__.py` & `kubemarine-0.29.0/kubemarine/templates/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/templates/plugins/calico-ippool.yaml.j2` & `kubemarine-0.29.0/kubemarine/templates/plugins/calico-ippool.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/templates/plugins/calico-rr.yaml.j2` & `kubemarine-0.29.0/kubemarine/templates/plugins/calico-rr.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/templates/plugins/dashboard-v2.5.yaml.j2` & `kubemarine-0.29.0/kubemarine/templates/plugins/dashboard-v2.5.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/templates/plugins/dashboard-v2.7.yaml.j2` & `kubemarine-0.29.0/kubemarine/templates/plugins/dashboard-v2.7.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/templates/plugins/iperf3.yaml.j2` & `kubemarine-0.29.0/kubemarine/templates/plugins/iperf3.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/templates/plugins/local-path-provisioner.yaml.j2` & `kubemarine-0.29.0/kubemarine/templates/plugins/local-path-provisioner.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/templates/plugins/nginx-ingress-controller-v1.2.yaml.j2` & `kubemarine-0.29.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.2.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/templates/plugins/nginx-ingress-controller-v1.4.yaml.j2` & `kubemarine-0.29.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.4.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine/testsuite.py` & `kubemarine-0.29.0/kubemarine/testsuite.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import io
 import textwrap
-from traceback import *
+from traceback import print_exc
 import csv
 from datetime import datetime
 from types import TracebackType
 from typing import Dict, Optional, Type, Union, List
 
 from kubemarine.core import utils, log
 
@@ -40,33 +40,33 @@
 
 
 class TestCase:
 
     def __enter__(self) -> 'TestCase':
         return self
 
-    def __exit__(self, type: Optional[Type[Exception]], value: Optional[Exception],
+    def __exit__(self, _: Optional[Type[Exception]], value: Optional[Exception],
                  traceback: Optional[TracebackType]) -> bool:
         if value is None:
             if self.status is TC_UNKNOWN:
                 self.success()
         elif isinstance(value, TestFailure):
             self.fail(value)
         elif isinstance(value, TestWarn):
             self.warn(value)
         else:
             self.exception(value)
-        print(self.get_summary(show_hint=True))
+        print(self.get_summary(show_hint=True))  # pylint: disable=bad-builtin
         return True
 
-    def __init__(self, cluster: KubernetesCluster, id: str, category: str, name: str,
+    def __init__(self, cluster: KubernetesCluster, id_: str, category: str, name: str,
                  default_results: str = None, minimal: int = None, recommended: int = None):
         self.include_in_ts(cluster.context['testsuite'])
         self.category = category
-        self.id = str(id)
+        self.id = str(id_)
         self.name = name
         self.status = TC_UNKNOWN
         self.results: Union[str, BaseException, None] = default_results
         self.minimal = minimal
         self.recommended = recommended
         self.cluster = cluster
 
@@ -148,15 +148,15 @@
         if show_recommended:
             if self.recommended is None:
                 output += ' ' * 14
             else:
                 recommended = str(self.recommended)
                 output += ' ' * (14-len(recommended)) + recommended
 
-        if show_hint and (isinstance(self.results, TestFailure) or isinstance(self.results, TestWarn)) and self.results.hint is not None:
+        if (show_hint and isinstance(self.results, (TestFailure, TestWarn)) and self.results.hint is not None):
             output += "\n                  HINT:\n" + textwrap.indent(str(self.results.hint), "                       ")
 
         return output
 
     def check_color(self) -> bool:
         for handler in self.cluster.log.handlers:
             if isinstance(handler, log.StdoutHandler) and handler.formatter.colorize:
@@ -220,54 +220,58 @@
 
     def is_any_test_warned(self) -> bool:
         for tc in self.tcs:
             if tc.is_warned():
                 return True
         return False
 
-    def get_final_summary(self, show_minimal: bool = True, show_recommended: bool = True) -> str:
+    def print_final_summary(self, show_minimal: bool = True, show_recommended: bool = True) -> None:
+        # pylint: disable-next=line-too-long
         result = "          Group    Status   ID    Test                                                               Actual result"
         if show_minimal:
             result += "        Minimal"
         if show_recommended:
             result += "   Recommended"
         result += "\n"
 
+        colorize = False
         for tc in self.tcs:
             result += "\n" + tc.get_summary(show_minimal=show_minimal, show_recommended=show_recommended)
+            colorize = tc.check_color()
 
         result += "\n\nOVERALL RESULTS: "
 
         for key, value in sorted(self.get_stats_data().items(), key=lambda _key: badges_weights[_key[0]]):
             colors = ''
-            if tc.check_color():
+            if colorize:
                 if key == 'succeeded':
                     colors = "\x1b[48;5;041m\x1b[38;5;232m"
                 if key == 'failed':
                     colors = "\x1b[48;5;196m\x1b[38;5;231m"
                 if key == 'warned':
                     colors = "\x1b[48;5;208m\x1b[38;5;231m"
                 if key == 'excepted':
                     colors = "\x1b[41m"
                 result += "%s %s %s \x1b[49m\x1b[39m " % (colors, value ,key.upper())
             else:
                 result += "%s %s  " % (value ,key.upper())
 
         result += "\n"
 
-        return result
+        print(result)  # pylint: disable=bad-builtin
 
     def print_final_status(self, logger: log.EnhancedLogger) -> None:
         if self.is_any_test_failed():
             logger.error("\nTEST FAILED"
                       "\nThe environment does not meet the minimal requirements. Check the test report and resolve the issues.")
             return
         if self.is_any_test_warned():
             logger.warning("\nTEST PASSED WITH WARNINGS"
-                        "\nThe environment meets the minimal requirements, but is not as recommended. Try to check the test report and resolve the issues.")
+                           "\nThe environment meets the minimal requirements, but is not as recommended. "
+                           "Try to check the test report and resolve the issues.")
             return
         logger.info("\nTEST PASSED")
 
     def get_stats_data(self) -> Dict[str, int]:
         results: Dict[str, int] = {}
         for tc in self.tcs:
             key = 'unknown'
@@ -300,27 +304,30 @@
             ])
 
         utils.dump_file({}, stream, destination_file_path, dump_location=False)
 
     def save_html(self, destination_file_path: str, check_type: str, append_styles: bool = True) -> None:
         stream = io.StringIO()
 
-        stream.write('<!DOCTYPE html><html><head><meta charset="utf-8"><title>%s Check Report</title></head><body><div id="date">%s</div><div id="stats">' % (check_type, datetime.utcnow()))
+        stream.write(f'<!DOCTYPE html><html><head><meta charset="utf-8"><title>{check_type} Check Report</title></head>'
+                     f'<body><div id="date">{datetime.utcnow()}</div><div id="stats">')
         for key, value in sorted(self.get_stats_data().items(), key=lambda _key: badges_weights[_key[0]]):
             stream.write('<div class="%s">%s %s</div>' % (key, value, key))
         stream.write('</div><h1>%s Check Report</h1><table>' % check_type)
-        stream.write('<thead><tr><td>Group</td><td>Status</td><td>ID</td><td>Test</td><td>Actual Result</td><td>Minimal</td><td>Recommended</td></tr></thead><tbody>')
+        stream.write('<thead><tr><td>Group</td><td>Status</td><td>ID</td><td>Test</td>'
+                     '<td>Actual Result</td><td>Minimal</td><td>Recommended</td></tr></thead><tbody>')
         for tc in self.tcs:
             minimal = ''
             if tc.minimal is not None:
                 minimal = str(tc.minimal)
             recommended = ''
             if tc.recommended is not None:
                 recommended = str(tc.recommended)
-            stream.write('<tr class="%s"><td>%s</td><td><div>%s</div></td><td>%s</td><td>%s</td><td>%s</td><td>%s</td><td>%s</td></tr>' %
+            stream.write('<tr class="%s"><td>%s</td><td><div>%s</div></td>'
+                         '<td>%s</td><td>%s</td><td>%s</td><td>%s</td><td>%s</td></tr>' %
                          (tc.get_readable_status(),
                           tc.category.lower(),
                           tc.get_readable_status(),
                           tc.id,
                           tc.name,
                           tc.results,
                           minimal,
```

### Comparing `kubemarine-0.28.1/kubemarine/thirdparties.py` & `kubemarine-0.29.0/kubemarine/thirdparties.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,16 +98,16 @@
 
 
 def get_thirdparty_destination(software_name: str) -> str:
     destination: str
     for destination, thirdparty_settings in static.GLOBALS['thirdparties'].items():
         if thirdparty_settings['software_name'] == software_name:
             return destination
-    else:
-        raise Exception(f"Failed to find third-party destination for {software_name!r}")
+
+    raise Exception(f"Failed to find third-party destination for {software_name!r}")
 
 
 def get_thirdparty_recommended_sha(destination: str, cluster: KubernetesCluster) -> Optional[str]:
     if not is_default_thirdparty(destination):
         # 3rd-party is not managed by Kubemarine
         return None
 
@@ -279,15 +279,15 @@
                 config['sha1'] = sha1
 
     # remove "crictl" from thirdparties when docker is used, but ONLY IF it is NOT explicitly specified in cluster.yaml
     cri_name = inventory['services']['cri']['containerRuntime']
     crictl_key = '/usr/bin/crictl.tar.gz'
     if cri_name == "docker" and \
             crictl_key not in cluster.raw_inventory.get('services', {}).get('thirdparties', {}):
-        del(thirdparties[crictl_key])
+        del thirdparties[crictl_key]
 
 
 def get_install_group(cluster: KubernetesCluster, config: dict) -> NodeGroup:
     return cluster.create_group_from_groups_nodes_names(
         config.get('groups', []), config.get('nodes', []))
 
 
@@ -341,15 +341,16 @@
     if is_curl:
         cluster.log.verbose('Installation via curl download detected')
         if config.get('sha1') is not None:
             cluster.log.verbose('SHA1 hash is defined, it will be used during installation')
             # if hash equal, then stop further actions immediately! unpack should not be performed too
             remote_commands += ' && FILE_HASH=$(sudo openssl sha1 %s | sed "s/^.* //"); ' \
                                '[ "%s" == "${FILE_HASH}" ] && exit 0 || true ' % (destination, config['sha1'])
-        remote_commands += ' && sudo rm -f %s && sudo curl --max-time %d -f -g -L %s -o %s && ' % (destination, cluster.inventory['globals']['timeout_download'], config['source'], destination)
+        remote_commands += (' && sudo rm -f %s && sudo curl --max-time %d -k -f -g -L %s -o %s && '
+                            % (destination, cluster.inventory['globals']['timeout_download'], config['source'], destination))
     else:
         cluster.log.verbose('Installation via sftp upload detected')
         cluster.log.debug(common_group.sudo(remote_commands))
         remote_commands = ''
         # TODO: Possible use SHA1 from inventory instead of calculating if provided?
         script = utils.read_internal(config['source'])
         common_group.put(io.StringIO(script), destination, sudo=True)
@@ -370,15 +371,16 @@
             cluster.log.verbose('Unzip will be used for unpacking')
             remote_commands += ' && sudo unzip -o %s -d %s' % (destination, config['unpack'])
             
             remote_commands += ' && sudo unzip -qq -l %s | awk \'NF > 3 { print $4 }\'| xargs -I FILE sudo chmod %s %s/FILE' \
                    % (destination, config['mode'], config['unpack'])
             remote_commands += ' && sudo unzip -qq -l %s | awk \'NF > 3 { print $4 }\'| xargs -I FILE sudo chown -R %s %s/FILE' \
                    % (destination, config['owner'], config['unpack'])
-            remote_commands += ' && sudo unzip -qq -l %s | awk \'NF > 3 { print $4 }\'| xargs -I FILE sudo ls -la %s/FILE' % (destination, config['unpack'])
+            remote_commands += ' && sudo unzip -qq -l %s | awk \'NF > 3 { print $4 }\'| xargs -I FILE sudo ls -la %s/FILE' \
+                   % (destination, config['unpack'])
             
         else:
             cluster.log.verbose('Tar will be used for unpacking')
             remote_commands += ' && sudo tar -zxf %s -C %s' % (destination, config['unpack'])
             
             remote_commands += ' && sudo tar -tf %s | xargs -I FILE sudo chmod %s %s/FILE' \
                            % (destination, config['mode'], config['unpack'])
```

### Comparing `kubemarine-0.28.1/kubemarine/yum.py` & `kubemarine-0.29.0/kubemarine/yum.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.1/kubemarine.egg-info/PKG-INFO` & `kubemarine-0.29.0/kubemarine.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubemarine
-Version: 0.28.1
+Version: 0.29.0
 Summary: Management tool for Kubernetes cluster deployment and maintenance
 Home-page: https://github.com/Netcracker/KubeMarine
 Author-email: Kubemarine Group <kubemarinegroup@netcracker.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Netcracker/KubeMarine
 Project-URL: Documentation, https://github.com/Netcracker/KubeMarine#documentation
 Project-URL: Issues, https://github.com/Netcracker/KubeMarine/issues/
@@ -49,50 +49,52 @@
 Requires-Dist: types-PyYAML==6.*; extra == "mypy"
 Requires-Dist: types-invoke==2.*; extra == "mypy"
 Requires-Dist: types-toml==0.*; extra == "mypy"
 Requires-Dist: types-python-dateutil==2.*; extra == "mypy"
 Requires-Dist: types-paramiko==3.*; extra == "mypy"
 Requires-Dist: types-jsonschema==4.*; extra == "mypy"
 Requires-Dist: types-pyinstaller==6.2.0.*; extra == "mypy"
+Provides-Extra: pylint
+Requires-Dist: pylint==3.1.*; extra == "pylint"
 
 ![Kubemarine_1280х640_3_JPEG](https://user-images.githubusercontent.com/5212888/162978291-63d55f19-7dc0-4126-ad39-cd69191e7e19.jpg)
 [![GitHub stars](https://img.shields.io/github/v/release/Netcracker/Kubemarine)](https://github.com/Netcracker/KubeMarine/releases)
 [![GitHub stars](https://img.shields.io/badge/contributions-welcome-orange.svg)](https://github.com/Netcracker/KubeMarine/blob/main/CONTRIBUTING.md)
 [![PyPI version](https://badge.fury.io/py/kubemarine.svg)](https://badge.fury.io/py/kubemarine)
 
 # Kubemarine
 
 Kubemarine is an open source, lightweight and powerful management tool built for end-to-end Kubernetes cluster deployment and maintenance. It is applicable for many purposes like simple and quick onboarding Kubernetes on local and production environments in different HA schemes depending on your aims, budget, and capabilities. Together with simplicity, Kubemarine can be a very flexible and customizable tool covering specific configurability cases on both deployment and maintenance stages. This library provides powerful CLI commands, as well as can be customized using a Python extension API.
 
 ## Highlights
 - Easy to use
-- Many procedures supported following the [generic maintenance approach](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#basics):
-  - [install](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#)
-  - [add_node](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#add-node-procedure)
-  - [remove_node](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#remove-node-procedure)
-  - [upgrade](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#upgrade-procedure)
-  - [backup](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#backup-procedure)
-  - [restore](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#restore-procedure)
-  - [reconfigure](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#reconfigure-procedure)
-  - [check_iaas](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Kubecheck.md#iaas-procedure)
-  - [check_paas](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Kubecheck.md#paas-procedure)
-  - [migrate_kubemarine](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#kubemarine-migration-procedure)
-  - [manage_psp](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#manage-psp-procedure)
-  - [manage_pss](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#manage-pss-procedure)
-  - [cert_renew](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#certificate-renew-procedure)
-  - [migrate_cri](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#cri-migration-procedure)
-- [Single cluster inventory](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#configuration) for all operations, highly customizable
+- Many procedures supported following the [generic maintenance approach](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#basics):
+  - [install](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#)
+  - [add_node](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#add-node-procedure)
+  - [remove_node](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#remove-node-procedure)
+  - [upgrade](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#upgrade-procedure)
+  - [backup](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#backup-procedure)
+  - [restore](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#restore-procedure)
+  - [reconfigure](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#reconfigure-procedure)
+  - [check_iaas](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Kubecheck.md#iaas-procedure)
+  - [check_paas](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Kubecheck.md#paas-procedure)
+  - [migrate_kubemarine](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#kubemarine-migration-procedure)
+  - [manage_psp](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#manage-psp-procedure)
+  - [manage_pss](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#manage-pss-procedure)
+  - [cert_renew](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#certificate-renew-procedure)
+  - [migrate_cri](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#cri-migration-procedure)
+- [Single cluster inventory](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#configuration) for all operations, highly customizable
 - Default values of all parameters in configurations with a minimum of required parameters
-- [Control planes balancing](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#full-ha-scheme) with external balancers and VRRP
-- Ability to [resume or skip specific task](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#tasks-list-redefinition) without re-running entire pipeline
-- [Pre-built plugins](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#predefined-plugins) out of the box and [custom plugins](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#custom-plugins-installation-procedures) support
-- Support for [executing in closed environments](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#installation-without-internet-resources) with private registries
-- Extended [logging](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Logging.md), configs [dumping](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#dump-files)
+- [Control planes balancing](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#full-ha-scheme) with external balancers and VRRP
+- Ability to [resume or skip specific task](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#tasks-list-redefinition) without re-running entire pipeline
+- [Pre-built plugins](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#predefined-plugins) out of the box and [custom plugins](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#custom-plugins-installation-procedures) support
+- Support for [executing in closed environments](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#installation-without-internet-resources) with private registries
+- Extended [logging](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Logging.md), configs [dumping](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#dump-files)
 - Build supported as a package, container, and binary
-- Package extension with [open extension API](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/PackageExtension.md)
+- Package extension with [open extension API](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/PackageExtension.md)
 - Support different deployment schemes (all-in-one, mini-HA, HA, and so on)
 
 ## Kubemarine Binary Installation
 Proceed the following steps to install Kubemarine  on your environment:
 1. Download the binary file for your system from the latest [release](https://github.com/Netcracker/KubeMarine/releases)
 2. Move binary kubemarine to a separate folder 
 3. Now you can proceed to run Kubemarine! Try the following:
@@ -110,15 +112,15 @@
    ```bash
    python3 -m pip install --upgrade pip
    ```
    Windows:
    ```bash
    python -m pip install --upgrade pip
    ```
-1. Ensure your environment meets the [Deployment Node Prerequisites](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#prerequisites-for-deployment-node).
+1. Ensure your environment meets the [Deployment Node Prerequisites](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#prerequisites-for-deployment-node).
 1. Create and activate a [virtual environment](https://realpython.com/python-virtual-environments-a-primer/) if necessary.
 1. Install Kubemarine package.
 
    Linux / MacOS:
    ```bash
    python3 -m pip install kubemarine
    ```
@@ -129,15 +131,15 @@
 1. Now you can proceed to run Kubemarine! Try the following:
    ```bash
    kubemarine help
    ```
 
 
 ## Kubemarine Installation from Sources
-Installation of Kubemarine from sources is mostly similar to [Kubemarine Package Installation](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/README.md#kubemarine-package-installation).
+Installation of Kubemarine from sources is mostly similar to [Kubemarine Package Installation](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/README.md#kubemarine-package-installation).
 The exception is instead of installing the package from [PyPI](https://pypi.org/project/kubemarine/), do the following:
 1. [Download the latest release](https://github.com/netcracker/kubemarine/releases) or clone the repository:
    ```bash
    git clone https://github.com/netcracker/kubemarine.git
    ```
 1. Unpack the project from the archive if required:
    ```bash
@@ -158,24 +160,24 @@
    python -m pip install -e .
    ```
 1. Now you can proceed to run Kubemarine. Try the following:
     ```bash
     kubemarine help
     ```
 
-**Note**: Building from [Dockerfile](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/Dockerfile) is also available.
+**Note**: Building from [Dockerfile](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/Dockerfile) is also available.
 
 
 **Note:** Kubemarine debugging available via `kubemarine/__main__.py`.
 
 
 ## Running Cluster Installation
 To install a Kubernetes cluster using Kubemarine:
-1. Prepare your VMs or bare-metal machines according to [Recommended Hardware Requirements](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#recommended-hardware-requirements) and the selected [Deployment Scheme](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#deployment-schemes). Make sure the nodes meet [Cluster Nodes Prerequisites](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#prerequisites-for-cluster-nodes).
-1. Create the `cluster.yaml` inventory file, and describe your environment. Make sure that all configurations are done. For more information, see [inventory configs available](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#configuration) and [examples](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/examples/cluster.yaml). No need to enter all the parameters that are available, it is enough to specify the minimal identification data about the nodes where you want to install the cluster, for example:
+1. Prepare your VMs or bare-metal machines according to [Recommended Hardware Requirements](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#recommended-hardware-requirements) and the selected [Deployment Scheme](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#deployment-schemes). Make sure the nodes meet [Cluster Nodes Prerequisites](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#prerequisites-for-cluster-nodes).
+1. Create the `cluster.yaml` inventory file, and describe your environment. Make sure that all configurations are done. For more information, see [inventory configs available](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#configuration) and [examples](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/examples/cluster.yaml). No need to enter all the parameters that are available, it is enough to specify the minimal identification data about the nodes where you want to install the cluster, for example:
    ```yaml
    node_defaults:
      keyfile: "/home/username/.ssh/id_rsa"
      password: '{{ env.PASS }}'     #Either keyfile or password can be used.
      username: "centos"
 
    vrrp_ips:
@@ -204,42 +206,42 @@
    kubemarine install
    ```
 1. Check the health of the newly installed cluster:
    ```bash
    kubemarine check_paas
    ```
 
-For more information, refer to the other [Kubemarine guides](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/README.md#documentation).
+For more information, refer to the other [Kubemarine guides](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/README.md#documentation).
 
 ## Kubemarine Docker Installation
 To start, download the Kubmarine image ```docker pull ghcr.io/netcracker/kubemarine:main```
 
 Run Kubemarine from the container, for example:
    ```
    docker run -it --mount type=bind,source=/root/cluster.yaml,target=/opt/kubemarine/cluster.yaml --mount type=bind,source=/root/rsa_key,target=/opt/kubemarine/rsa_key kubemarine install -c /opt/kubemarine/cluster.yaml
    ```
    *Note*: Do not forget to pass the inventory file and connection key inside the container.
    For more execution details, refer to ["Installation of Kubernetes using CLI" guide on Github](https://github.com/Netcracker/kubemarine/blob/main/documentation/Installation.md#installation-of-kubernetes-using-cli).
 
 ## Documentation
 The following documents and tutorials are available:
-- [Installation](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md)
-- [Maintenance](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md)
-- [Troubleshooting](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Troubleshooting.md)
-- [Kubecheck](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Kubecheck.md)
-- [Logging](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Logging.md)
+- [Installation](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md)
+- [Maintenance](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md)
+- [Troubleshooting](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Troubleshooting.md)
+- [Kubecheck](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Kubecheck.md)
+- [Logging](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Logging.md)
 
 Also, check out the following inventory examples:
-- [cluster.yaml](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/examples/cluster.yaml)
-- [procedure.yaml](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/examples/procedure.yaml)
+- [cluster.yaml](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/examples/cluster.yaml)
+- [procedure.yaml](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/examples/procedure.yaml)
 
 ## Issues, Questions
 If you have any problems while working with Kubemarine, feel free to open a [new issue](https://github.com/netcracker/kubemarine/issues) or even
 [PR](https://github.com/netcracker/kubemarine/pulls) with related changes.
-Please follow the [Contribution Guide](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/CONTRIBUTING.md ) and the process outlined in the Stack Overflow [MCVE](https://stackoverflow.com/help/mcve) document.
+Please follow the [Contribution Guide](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/CONTRIBUTING.md ) and the process outlined in the Stack Overflow [MCVE](https://stackoverflow.com/help/mcve) document.
 
-In case of security concerns, please follow the [Security Reporting Process](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/SECURITY.md)
+In case of security concerns, please follow the [Security Reporting Process](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/SECURITY.md)
 ## Changelog
 Detailed changes for each release are documented in the [release notes](https://github.com/netcracker/kubemarine/releases).
 
 ## License
-[Apache License 2.0](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/LICENSE)
+[Apache License 2.0](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/LICENSE)
```

### Comparing `kubemarine-0.28.1/kubemarine.egg-info/SOURCES.txt` & `kubemarine-0.29.0/kubemarine.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -64,16 +64,17 @@
 kubemarine/kubernetes/daemonset.py
 kubemarine/kubernetes/deployment.py
 kubemarine/kubernetes/object.py
 kubemarine/kubernetes/replicaset.py
 kubemarine/kubernetes/secrets.py
 kubemarine/kubernetes/statefulset.py
 kubemarine/patches/__init__.py
-kubemarine/patches/patch_kubelet_configmap.py
+kubemarine/patches/boot_timeout_per_node.py
 kubemarine/patches/software_upgrade.yaml
+kubemarine/patches/strong_cipher_suits_for_kubelet.py
 kubemarine/plugins/__init__.py
 kubemarine/plugins/builtin.py
 kubemarine/plugins/calico.py
 kubemarine/plugins/kubernetes_dashboard.py
 kubemarine/plugins/local_path_provisioner.py
 kubemarine/plugins/manifest.py
 kubemarine/plugins/nginx_ingress.py
@@ -98,14 +99,15 @@
 kubemarine/plugins/yaml/nginx-ingress-controller-v1.2.0-original.yaml
 kubemarine/plugins/yaml/nginx-ingress-controller-v1.4.0-original.yaml
 kubemarine/plugins/yaml/nginx-ingress-controller-v1.7.0-original.yaml
 kubemarine/plugins/yaml/nginx-ingress-controller-v1.8.1-original.yaml
 kubemarine/plugins/yaml/nginx-ingress-controller-v1.8.4-original.yaml
 kubemarine/plugins/yaml/nginx-ingress-controller-v1.9.4-original.yaml
 kubemarine/plugins/yaml/nginx-ingress-controller-v1.9.5-original.yaml
+kubemarine/plugins/yaml/nginx-ingress-controller-v1.9.6-original.yaml
 kubemarine/procedures/__init__.py
 kubemarine/procedures/add_node.py
 kubemarine/procedures/backup.py
 kubemarine/procedures/cert_renew.py
 kubemarine/procedures/check_iaas.py
 kubemarine/procedures/check_paas.py
 kubemarine/procedures/config.py
@@ -198,14 +200,15 @@
 kubemarine/resources/schemas/definitions/services/modprobe.json
 kubemarine/resources/schemas/definitions/services/ntp.json
 kubemarine/resources/schemas/definitions/services/packages.json
 kubemarine/resources/schemas/definitions/services/resolv.conf.json
 kubemarine/resources/schemas/definitions/services/sysctl.json
 kubemarine/resources/schemas/definitions/services/thirdparties.json
 kubemarine/resources/schemas/definitions/services/packages/associations.json
+kubemarine/resources/schemas/internal/connections.json
 kubemarine/resources/scripts/__init__.py
 kubemarine/resources/scripts/check_haproxy.sh
 kubemarine/resources/scripts/check_url_availability.py
 kubemarine/resources/scripts/etcdctl.sh
 kubemarine/resources/scripts/ipip_check.gz
 kubemarine/resources/scripts/simple_port_client.py
 kubemarine/resources/scripts/simple_port_listener.py
```

### Comparing `kubemarine-0.28.1/setup.py` & `kubemarine-0.29.0/setup.py`

 * *Files identical despite different names*

