# Simple Symfony Console wrapper 
Catch all exceptions and write message, trace (in verbose mode) to console output. 

Returns code depends of executing result. Zero on success. Exception code or one otherwise. 

[![Software License][badge-license]][license]

## Installation
```bash
composer require sbooker/console
```
## Usage
```php
use Sbooker\Console\Command;
use Symfony\Component\Console\Input\InputInterface;
use Symfony\Component\Console\Output\OutputInterface;

class ConcreteCommand extends Command
{
    // Define command. See [Symfony Console Component](https://symfony.com/doc/current/components/console.html) 

    protected function doExecute(InputInterface $input, OutputInterface $output) : void {
        // .... do something successful ....
    }
}
```
## License
See [LICENSE][license] file.

[badge-license]: https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square
[license]: https://github.com/sbooker/console/blob/master/LICENSE

