# Log4net config example

```C#
	class Program
    {
        static void Main(string[] args)
        {
            log4net.Config.XmlConfigurator.Configure();

            var logger = LogManager.GetLogger(typeof (Program));

            logger.Info("Hello world");

        }
    }

```

or add to assembly default config

```C#
[assembly: log4net.Config.XmlConfigurator]
```