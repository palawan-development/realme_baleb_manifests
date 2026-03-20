# realme GT Neo6 manifests

### Available branches
- `lineage-23.2`

### How to use

**Create ROM directory and initialize it's repository (if you haven't done that yet)**
```bash
mkdir -p LineageOS; cd LineageOS
repo init \
-u https://github.com/LineageOS/android.git \
-b lineage-<version> \
--git-lfs
```

**Clone manifest**
```bash
git clone https://github.com/palawan-development/realme_bale-b_manifests.git .repo/local_manifests \
-b <specified-branch>
```

**Sync**
```bash
repo sync \
--no-clone-bundle \
--prune \
--force-sync \
--optimized-fetch \
--no-tags \
--retry-fetches=5 \
-j6
```

**Done! All repositories from the manifest should be synchronized**
