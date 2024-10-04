
# JSON Structure Description

## Report Metadata
- **report_version**: Version of the report (e.g., "2.0").

## System Information
- **hostname**: The network name of the machine (e.g., "HOST-123").
- **domain**: Domain the machine belongs to (e.g., "mfc.ru").
- **uuid**: Universally unique identifier (UUID) of the Windows system (e.g., "123e4567-e89b-12d3-a456-426614174000").

## Technical Information
- **tech**:
  - **cpu**: List of CPUs installed on the system. Example:
    - "Intel(R) Core(TM) i5-2400"
    - "Intel Xeon E5 2630"
  - **videoadapter**: List of video adapters (GPUs) installed. Example:
    - "Intel(R) UHD Graphics 630"
    - "NVIDIA GeForce GTX 1050 TI"
  - **cd_dvd**: Information about the CD/DVD drive (currently not used).
  - **motherboard**:
    - **vendor**: The vendor of the motherboard (e.g., "ASUS").
    - **model**: The model of the motherboard (e.g., "PRIME H410M-K R2.0").
  - **os**:
    - **windows**:
      - **small**: Short description of the Windows operating system (e.g., "Microsoft Windows 10 Pro").
      - **full**: Detailed description of the Windows version (e.g., "Microsoft Windows 10 Pro 10.0.19042.631 (Win10 20H2 October 2020 Update)").
    - **linux**:
      - **name**: Name of the Linux distribution (e.g., "Debian GNU/Linux 10").
      - **version**: Version of the Linux distribution (e.g., "10.1").
      - **core**: Kernel version of the Linux system (e.g., "Linux 5.18.14-arch1-1 x86_64").
  - **ram**: Total amount of RAM installed (e.g., "16 ГБ").
  - **disk**: List of disk drives. Each disk includes:
    - **model**: Model of the disk (e.g., "TEAM TM8FP6256G").
    - **size**: Disk size (e.g., "256 ГБ").
    - **mediatype**: Media type (e.g., "Fixed hard disk media").

## Peripherals
- **per**:
  - **monitor**: List of monitor vendors (e.g., "Dell").
  - **keyboard**: Vendor of the keyboard (e.g., "Logitech").
  - **mouse**: Vendor of the mouse (e.g., "Razer").

## Organizational Information
- **org**:
  - **type_arm**: Type of machine, either "serv" (server) or "arm" (workstation).
  - **inventory**: Inventory number of the system (e.g., "INV-123456").
  - **cabinet**: Cabinet or room information where the machine is located, as an array:
    - Room name (e.g., "Кабинет №5").
    - Address (e.g., "228288, СПБ, улица Пушкина, дом Колотушкина").
  - **empl**: List of employees associated with the machine. Each entry includes:
    - **full_name**: Full name of the employee (e.g., "Иванов Иван Иванович").
    - **position**: Job position (e.g., "Системный администратор").
    - **structural**: Department or structural unit (e.g., "IT отдел").

## Network Interfaces
- **interfaces**:
  - **name**: Name of the network interface (e.g., "eth0").
  - **state**: Whether the interface is active (true/false).
  - **ipv4**: List of IPv4 addresses and subnet masks.
    - **address**: IPv4 address (e.g., "192.168.0.1").
    - **subnet**: Subnet mask (e.g., "255.255.255.0").
  - **mac**: List of MAC addresses (e.g., "00:1A:2B:3C:4D:5E").

## Installed Applications
- **app_list**: List of installed applications. Each entry includes:
  - **name**: Name of the application (e.g., "KES").
  - **version**: Version of the application (e.g., "1.0.0").
  - **data_install**: Installation date (e.g., "2023-01-15").
