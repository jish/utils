require 'fileutils'

class Installer
  def install
    files.each do |src|
      dest = "~/#{src}"

      source = File.expand_path(src)
      destination = File.expand_path(dest)

      FileUtils.mkdir_p(File.dirname(destination))

      if File.exist?(destination)
        puts "#{dest} exists"
      else
        puts "Linking #{dest}"
        link(source, destination)
      end
    end
  end

  def files
    Dir['bin/*']
  end

  def link(source, destination)
    FileUtils.ln_s(source, destination)
  end

end

desc 'Install'
task :install do
  Installer.new.install
end
