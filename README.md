# halogen #130 data

Per-position files and logs for peonist-ai/halogen-flash-server#130 (Qwen3.8-Flash-Next quant comparisons on Strix Halo, halogen `ppl` mode).

Release `ht43-2026-10-03` holds `h130-ht43.tgz` (sha256 `6ec3e6a7bfa950aeeac456b22ad47586dfa2ce141d323eb35f9e874ffd5465ed`):

- `ht43-{wt2,zh,code}.pos`: ht43 `--per-pos` output against a v2 reference (16 bytes per position: f32 kl, dp, top1, nll)
- `v2-{wt2,zh,code}.nll.f32`: v2 per-position NLL, the `nll` field of each `--ref-out` record (the full reference dumps are 350-460 MB, available on request)
- `ud-wt2.pos`: UD-Q4_K_XL `--per-pos` from the earlier comparison in the issue (0.16.1, against the 0.16.1 v2 reference)
- `ht43-*.json`, `v2r-*.json`: the tool's own JSON output
- `paired.py`: the paired block statistic; `ht43-run.sh`, `ht43-run.log`: the exact run
