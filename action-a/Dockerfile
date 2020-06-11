From 45612c20be1754d32b4c91f815379aa7003b66e0 Mon Sep 17 00:00:00 2001
From: Matthew Davis <38021615+mattdavis0351@users.noreply.github.com>
Date: Thu, 24 Oct 2019 09:25:22 -0700
Subject: [PATCH 1/7] Update ci-workflow.yml

---
 .github/ci-workflow.yml | 2 ++
 1 file changed, 2 insertions(+)

diff --git a/.github/ci-workflow.yml b/.github/ci-workflow.yml
index 03a5d43..b8bd62c 100644
--- a/.github/ci-workflow.yml
+++ b/.github/ci-workflow.yml
@@ -1,3 +1,5 @@
+# This file wont do us much good in this location, make sure you change the path as directed to continue!
+
 name: Node CI
 
 on: [push]

From f45777923d017d5916cb345c93db0ea3b77f4f20 Mon Sep 17 00:00:00 2001
From: mattdavis0351 <mattdavis0351@github.com>
Date: Thu, 24 Oct 2019 14:30:43 -0700
Subject: [PATCH 2/7] updating workflow file

---
 .github/ci-workflow.yml | 7 +++++--
 1 file changed, 5 insertions(+), 2 deletions(-)

diff --git a/.github/ci-workflow.yml b/.github/ci-workflow.yml
index b8bd62c..963afa7 100644
--- a/.github/ci-workflow.yml
+++ b/.github/ci-workflow.yml
@@ -2,8 +2,11 @@
 
 name: Node CI
 
-on: [push]
-
+on:
+  push:
+    branches-ignore:
+      - "ci-workflow"
+      - "docker-workflow"
 jobs:
   build:
     runs-on: ubuntu-latest

From 9b71af726291a26db6fa1a3a8b9e7604cbfcbf28 Mon Sep 17 00:00:00 2001
From: mattdavis0351 <mattdavis0351@github.com>
Date: Thu, 24 Oct 2019 14:42:24 -0700
Subject: [PATCH 3/7] workflow trigger change"

---
 .github/ci-workflow.yml | 8 +++++---
 1 file changed, 5 insertions(+), 3 deletions(-)

diff --git a/.github/ci-workflow.yml b/.github/ci-workflow.yml
index 963afa7..cbffd59 100644
--- a/.github/ci-workflow.yml
+++ b/.github/ci-workflow.yml
@@ -4,9 +4,11 @@ name: Node CI
 
 on:
   push:
-    branches-ignore:
-      - "ci-workflow"
-      - "docker-workflow"
+    # branches-ignore:
+    #   - "ci-workflow"
+    #   - "docker-workflow"
+    paths-ignore:
+      - ".github/**"
 jobs:
   build:
     runs-on: ubuntu-latest

From f60fb057e7846b5e1344c7f7fe4cc8b8f2bb7735 Mon Sep 17 00:00:00 2001
From: mattdavis0351 <mattdavis0351@github.com>
Date: Thu, 24 Oct 2019 14:48:04 -0700
Subject: [PATCH 4/7] more path ignore

---
 .github/ci-workflow.yml | 1 +
 1 file changed, 1 insertion(+)

diff --git a/.github/ci-workflow.yml b/.github/ci-workflow.yml
index cbffd59..59a896a 100644
--- a/.github/ci-workflow.yml
+++ b/.github/ci-workflow.yml
@@ -9,6 +9,7 @@ on:
     #   - "docker-workflow"
     paths-ignore:
       - ".github/**"
+      - ".github/workflows/**"
 jobs:
   build:
     runs-on: ubuntu-latest

From ef8941e7cb16f5713e168a4f5f6d853b28ad9cca Mon Sep 17 00:00:00 2001
From: mattdavis0351 <mattdavis0351@github.com>
Date: Thu, 24 Oct 2019 14:56:56 -0700
Subject: [PATCH 5/7] workflow file update

---
 .github/ci-workflow.yml | 5 ++---
 1 file changed, 2 insertions(+), 3 deletions(-)

diff --git a/.github/ci-workflow.yml b/.github/ci-workflow.yml
index 59a896a..482b71f 100644
--- a/.github/ci-workflow.yml
+++ b/.github/ci-workflow.yml
@@ -7,9 +7,8 @@ on:
     # branches-ignore:
     #   - "ci-workflow"
     #   - "docker-workflow"
-    paths-ignore:
-      - ".github/**"
-      - ".github/workflows/**"
+    paths:
+      - "**Dockerfile**"
 jobs:
   build:
     runs-on: ubuntu-latest

From 0c6bf845018742d3c8761697b2a9bb1791fb44e6 Mon Sep 17 00:00:00 2001
From: Matthew Davis <38021615+mattdavis0351@users.noreply.github.com>
Date: Tue, 5 May 2020 12:19:56 -0700
Subject: [PATCH 6/7] Update ci-workflow.yml

---
 .github/ci-workflow.yml | 2 +-
 1 file changed, 1 insertion(+), 1 deletion(-)

diff --git a/.github/ci-workflow.yml b/.github/ci-workflow.yml
index 482b71f..a837433 100644
--- a/.github/ci-workflow.yml
+++ b/.github/ci-workflow.yml
@@ -29,7 +29,7 @@ jobs:
     strategy:
       matrix:
         os: [ubuntu-lastest, windows-2016]
-        node-version: [8.x, 10.x]
+        node-version: [10,12]
 
     steps:
       - uses: actions/checkout@v1

From aa88a3ac5decbcc4a99a67bdab508edad6aad434 Mon Sep 17 00:00:00 2001
From: Matthew Davis <38021615+mattdavis0351@users.noreply.github.com>
Date: Tue, 5 May 2020 12:21:05 -0700
Subject: [PATCH 7/7] Update ci-workflow.yml

---
 .github/ci-workflow.yml | 2 +-
 1 file changed, 1 insertion(+), 1 deletion(-)

diff --git a/.github/ci-workflow.yml b/.github/ci-workflow.yml
index a837433..883d6cc 100644
--- a/.github/ci-workflow.yml
+++ b/.github/ci-workflow.yml
@@ -29,7 +29,7 @@ jobs:
     strategy:
       matrix:
         os: [ubuntu-lastest, windows-2016]
-        node-version: [10,12]
+        node-version: [10, 12]
 
     steps:
       - uses: actions/checkout@v1
       
       diff --git a/.github/ci-workflow.yml b/.github/ci-workflow.yml
index 03a5d43..883d6cc 100644
--- a/.github/ci-workflow.yml
+++ b/.github/ci-workflow.yml
@@ -1,7 +1,14 @@
-name: Node CI
+# This file wont do us much good in this location, make sure you change the path as directed to continue!
 
-on: [push]
+name: Node CI
 
+on:
+  push:
+    # branches-ignore:
+    #   - "ci-workflow"
+    #   - "docker-workflow"
+    paths:
+      - "**Dockerfile**"
 jobs:
   build:
     runs-on: ubuntu-latest
@@ -22,7 +29,7 @@ jobs:
     strategy:
       matrix:
         os: [ubuntu-lastest, windows-2016]
-        node-version: [8.x, 10.x]
+        node-version: [10, 12]
 
     steps:
       - uses: actions/checkout@v1
