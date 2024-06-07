# Bug report for `poetry2nix`

There is a bug in `poetry2nix`

The following commands should all work fine:

1. ✅ `nix develop -c poetry run python -m foo`
2. ✅ `nix develop -c python -m foo`
3. ✅ `nix develop -c poetry run python -m bar`
4. ❌ `nix develop -c python -m bar`

Why does 4 fail with error `/nix/store/ax27bnhj64aba7ilab3jz4gpyvsym16i-python3-3.11.9-env/bin/python3.11: No module named bar`?
