Mini Windows XP loads with a 24 MB File.

Loading and unloading of ISO files is not supported on this basic stripped down system.


*Including Custom Programs in the MiniXP Image*

Due to the stripped-down nature of the MiniXP environment used in this project, adding your own programs requires a manual packaging step. This is a limitation of keeping the operating system extremely small and self-contained.

To include a custom application, you must first extract the compressed ISO image. The ISO is distributed in .gz format, so begin by unzipping it using a standard gzip-compatible tool.

Once extracted, open the ISO using an ISO editing utility such as PowerISO, UltraISO, or a similar tool. From there, you can inject your application files directly into the filesystem.

Optionally, if your application needs to launch automatically on boot, you may modify the Windows registry inside the image to configure auto-loading. This step is not required for all programs and should be done carefully.

After making your changes, save the modified ISO and recompress it using gzip. The resulting .iso.gz file can then be referenced by the web-based loader HTML used by this project.
Why This Approach Exists

This workflow exists because the MiniXP image is intentionally minimal. The goal is to achieve an extremely small download size while still providing a functional Windows XP live environment.

The result is a footprint comparable to archive.org-style DOSBox environments that boot lightweight Windows setups — except this project runs a Windows XP live environment directly in the browser using v86.

While traditional DOSBox-based Windows 3.1 setups are often choppy, buggy, and slow, this approach achieves similar functionality with better responsiveness, at the cost of requiring more effort when packaging custom applications.

In practice, this means small applications can be bundled effectively, though compatibility is not guaranteed. Some trial and error is expected.
Recommendation

This MiniXP configuration should be viewed primarily as an interesting proof of concept. If you find the approach compelling and want a more practical setup, it is recommended to use the standard v86 Windows XP loader instead.

The full loader uses a larger image (approximately 90 MB), but in return it supports easy mounting of both local and remote ISO files and avoids many of the missing core operating system components present in the MiniXP build.

For most real-world use cases, the full v86 XP loader provides a smoother and more flexible experience.
