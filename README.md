# Learning C#

Just one of the things I'm learning. https://github.com/hchiam/learning

## Basics

https://www.learncs.org/

https://www.youtube.com/watch?v=udnsw1eMVOg&list=PLkX2tb_Jm6xqj9hZ8LczOHoSELIr5SXeU

https://www.tutorialspoint.com/csharp/index.htm

## Get .NET to get C# to run in VSCode with `dotnet run`

https://dotnet.microsoft.com/en-us/download/dotnet/sdk-for-vs-code

https://learn.microsoft.com/en-us/dotnet/core/tutorials/with-visual-studio-code

```sh
mkdir HelloWorldExample
cd HelloWorldExample
dotnet new console --framework net7.0
# you can safely ignore the bin and obj folder - they're auto-generated when you run
```

```cs
namespace HelloWorld
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Hello, World!");
        }
    }
}
```

```sh
dotnet run
```

### To opt out of telemetry

Open .bash_profile:

```sh
source ~/.bash_profile
```

Add this to .bash_profile:

```txt
export DOTNET_CLI_TELEMETRY_OPTOUT=1
```

Check that it worked: (should print out 1)

```sh
echo $DOTNET_CLI_TELEMETRY_OPTOUT
```
