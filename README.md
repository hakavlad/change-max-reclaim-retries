
# Replace MAX_RECLAIM_RETRIES by vm.max_reclaim_retries

This patch replaces `MAX_RECLAIM_RETRIES` in `mm/internal.h` by a new 
sysctl knob `vm.max_reclaim_retries`.

This patch may be correctly applied (at least) to Linux 5.4—5.12-rc2.

Default `vm.max_reclaim_retries` value can be changed via `CONFIG_MAX_RECLAIM_RETRIES`.

There are two versions with different default values:
- `Change_max_reclaim_retries_16_5.10.patch` provides `vm.max_reclaim_retries` with default value 16;
- `Change_max_reclaim_retries_0_5.10.patch` provides `vm.max_reclaim_retries` with default value 0.
