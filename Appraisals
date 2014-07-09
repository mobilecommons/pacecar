rails_versions = %w(4.0 4.1)
databases = %w(mysql2 pg sqlite3)

rails_versions.each do |rails_version|
  databases.each do |database|
    appraise "rails_#{rails_version}_#{database}_driver" do
      gem 'rails', rails_version
      gem database
    end
  end
end
