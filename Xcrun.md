usage: simctl [--noxpc] [--set <path>] [--profiles <path>] <subcommand> ...
       simctl help [subcommand]
Command line utility to control the Simulator

For subcommands that require a <device> argument, you may specify a device UDID
or the special "booted" string which will cause simctl to pick a booted device.
If multiple devices are booted when the "booted" device is selected, simctl
will choose one of them.

Subcommands:
	create              Create a new device.
	clone               Clone an existing device.
	upgrade             Upgrade a device to a newer runtime.
	delete              Delete a device or all unavailable devices.
	pair                Create a new watch and phone pair.
	unpair              Unpair a watch and phone pair.
	pair_activate       Set a given pair as active.
	erase               Erase a device's contents and settings.
	boot                Boot a device.
	shutdown            Shutdown a device.
	rename              Rename a device.
	getenv              Print an environment variable from a running device.
	openurl             Open a URL in a device.
	addmedia            Add photos, live photos, or videos to the photo library of a device.
	install             Install an app on a device.
	uninstall           Uninstall an app from a device.
	get_app_container   Print the path of the installed app's container
	launch              Launch an application by identifier on a device.
	terminate           Terminate an application by identifier on a device.
	spawn               Spawn a process on a device.
	list                List available devices, device types, runtimes, or device pairs.
	icloud_sync         Trigger iCloud sync on a device.
	pbsync              Sync the pasteboard content from one pasteboard to another.
	pbcopy              Copy standard input onto the device pasteboard.
	pbpaste             Print the contents of the device's pasteboard to standard output.
	help                Prints the usage for a given subcommand.
	io                  Set up a device IO operation.
	diagnose            Collect diagnostic information and logs.
	logverbose          enable or disable verbose logging for a device
