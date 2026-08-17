# fuzzy-parakeet

GitHub
│
├── platform-repo
│   ├── argocd
│   ├── ingress
│   └── monitoring
│
└── application-repo
    ├── base
    └── overlays
        ├── dev
        ├── test
        └── prod

            ↓

        Argo CD

            ↓

+----------------------+
|      k3d cluster     |
+----------------------+
| argocd namespace     |
| dev namespace        |
| test namespace       |
| prod namespace       |
+----------------------+
