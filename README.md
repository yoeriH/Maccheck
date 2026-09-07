# Maccheck

echo "=== HARDWARE ==="; system_profiler SPHardwareDataType SPPowerDataType | grep -E "Model Name:|Model Identifier:|Chip:|Memory:|Serial Number \(system\):|Activation Lock Status:|Cycle Count:|Maximum Capacity:|Condition:"; echo "=== MDM STATUS ==="; profiles status -type enrollment 2>&1; echo "=== ADE/DEP ==="; sudo profiles show -type enrollment 2>&1
