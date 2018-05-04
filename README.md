# 
Puppet module to manage NTP

# Install the module with r10k :

sudo r10k puppetfile install --verbose

# Puppetfile 
mod 'puppet_ntp',
  :git => 'https://github.com/louiekwan/puppet_ntp.git',
  :tag => '0.1.0'

sudo puppet apply --environment=lkwan -e 'include puppet_ntp'

# Check
timedatectl status
