# ProtectionIntegration

If you want to add a custom protection integration for your own plugin, you can do so by implementing the 
``ProtectionIntegration`` interface. This interface provides a handful of methods that will be called by the 
``ProtectionManager``.

For an example of how to implement this interface, you can check out some of our 
[built-in protection integrations](https://github.com/xenondevs/Nova/tree/main/Nova/src/main/kotlin/xyz/xenondevs/nova/integration/protection/plugin).

Once you have implemented the interface, you can register it with ``Nova.registerProtectionIntegration(ProtectionIntegration)``.

If you just want to block a specific action you can use the [``ProtectionCheckEvent``](../events/protectioncheckevent.md) instead.