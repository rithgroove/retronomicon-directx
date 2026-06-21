# retronomicon-directx

DirectX graphics backend boundary for Retronomicon.

The current CMake target, `retronomicon-directx`, is a placeholder interface so
the workspace can select `RETRONOMICON_GRAPHICS_BACKEND=DIRECTX` without
coupling DirectX code into the core engine. Add Win32 window, Direct3D renderer,
texture manager, and input implementations here.
