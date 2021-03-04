# Replace MAX_RECLAIM_RETRIES by vm.max_reclaim_retries

This patch replaces MAX_RECLAIM_RETRIES in `mm/internal.h` by a new 
sysctl knob `vm.max_reclaim_retries` with default value 16.
