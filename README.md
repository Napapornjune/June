import React from "react";

export default function HomePage() {
  return (
    <div className="font-sans">
      {/* Header */}
      <header className="bg-green-700 text-white p-4 flex justify-between items-center">
        <div className="flex items-center gap-4">
          <img
            src="/logo-moph.png"
            alt="โลโก้สาธารณสุข"
            className="h-12"
          />
          <div>
            <h1 className="text-xl font-bold">
              สำนักงานสาธารณสุขอำเภอวิหารแดง
            </h1>
            <p className="text-sm">District Health Office Wihan Daeng</p>
          </div>
        </div>
        <div className="space-x-2">
          <button className="bg-white text-green-700 px-2 py-1 rounded">TH</button>
          <button className="bg-white text-green-700 px-2 py-1 rounded">EN</button>
        </div>
      </header>

      {/* Navigation */}
      <nav className="bg-green-600 text-white px-6 py-2 flex gap-6 text-sm">
        <a href="#" className="hover:underline">หน้าแรก</a>
        <a href="#" className="hover:underline">เกี่ยวกับเรา</a>
        <a href="#" className="hover:underline">โครงสร้างองค์กร</a>
        <a href="#" className="hover:underline">สำหรับประชาชน</a>
        <a href="#" className="hover:underline">สำหรับเจ้าหน้าที่</a>
        <a href="#" className="hover:underline">ติดต่อเรา</a>
      </nav>

      {/* Hero Section */}
      <section className="p-8 bg-gray-50 text-center">
        <h2 className="text-2xl font-bold mb-2">
          ให้ข้อมูลเกี่ยวกับภารกิจ แผนงาน และกิจกรรมทางสาธารณสุข
        </h2>
        <p className="text-gray-600">
          บริการข้อมูลและข่าวสารสำหรับประชาชน
        </p>
      </section>

      {/* Content Sections */}
      <section className="grid grid-cols-1 md:grid-cols-3 gap-6 p-6">
        <div className="bg-white shadow rounded-2xl p-4">
          <h3 className="font-semibold mb-2">สำหรับประชาชน</h3>
          <p className="text-sm text-gray-600">
            แบบฟอร์มร้องขอใบรับบริการ เอกสารสําหรับขอข้อมูลข่าวสาร
          </p>
          <a href="#" className="text-blue-600 text-sm">ดาวน์โหลด (PDF)</a>
        </div>

        <div className="bg-white shadow rounded-2xl p-4">
          <h3 className="font-semibold mb-2">สำหรับเจ้าหน้าที่</h3>
          <p className="text-sm text-gray-600">
            เข้าสู่ระบบเอกสารภายใน หรือเข้าถึงทรัพยากรบุคลากร
          </p>
          <a href="#" className="text-blue-600 text-sm">เข้าสู่ระบบ</a>
        </div>

        <div className="bg-white shadow rounded-2xl p-4">
          <h3 className="font-semibold mb-2">ข่าวประชาสัมพันธ์</h3>
          <ul className="text-sm text-gray-600 list-disc list-inside">
            <li>กิจกรรมให้บริการฉีดวัคซีน - 18 เม.ย. 2567</li>
            <li>รณรงค์ไข้เลือดออก - 10 เม.ย. 2567</li>
            <li>ประชุมองค์กรสาธารณสุข - 25 มี.ค. 2567</li>
          </ul>
        </div>
      </section>

      {/* Contact Section */}
      <section className="p-6 bg-gray-100">
        <h3 className="text-lg font-bold mb-4">ติดต่อเรา</h3>
        <form className="grid grid-cols-1 md:grid-cols-2 gap-4 mb-6">
          <input
            type="text"
            placeholder="ชื่อ"
            className="border p-2 rounded"
          />
          <input
            type="email"
            placeholder="อีเมล"
            className="border p-2 rounded"
          />
          <textarea
            placeholder="ข้อความ"
            className="border p-2 rounded col-span-1 md:col-span-2"
            rows="4"
          ></textarea>
          <button className="bg-blue-600 text-white px-4 py-2 rounded col-span-1 md:col-span-2">
            ส่ง
          </button>
        </form>

        {/* Additional Contact Info */}
        <div className="text-sm text-gray-700">
          <p>โทรศัพท์: 036-123456</p>
          <p>โทรสาร: 036-654321</p>
          <p>อีเมล: vihandaeng@moph.go.th</p>
          <p>Facebook: <a href="https://facebook.com/vihandaenghealth" className="text-blue-600" target="_blank">สำนักงานสาธารณสุขอำเภอวิหารแดง</a></p>
        </div>
      </section>

      {/* Footer */}
      <footer className="bg-green-700 text-white text-sm text-center p-4">
        © 2025 สำนักงานสาธารณสุขอำเภอวิหารแดง
      </footer>
    </div>
  );
}
